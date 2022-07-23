##Useful readings about GIT related best practices (annotated):

- [Article "Best practices for teams. GIT"](https://opensource.com/article/20/7/git-best-practices):
  - GIT convention for the team should be formalized
  - Rebase feature branch 
often 
  ```
  git checkout master
  git pull
  git checkout feature-xyz  # name of your hypothetical feature branch
  git rebase master  # may need to fix merge conflicts in feature-xyz
  ```
  - Squash commits before merging. In general, there should only be one or a few commits added to master from each feature branch. To achieve this, squash multiple commits into one or a handful of commits with more elaborate messages for each one.
  ```
  git rebase -i HEAD~20  # look at up to 20 commits to consider squashing
  ```
    - Use tags to preserve the current state as a significant milestone. While a branch accumulates a history of changes corresponding to commits, a tag is a snapshot of the branch's state at that instant. A tag can be thought of as a history-less branch or as a named pointer to a specific commit immediately before the tag was created.