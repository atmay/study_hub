# cheetsheet
Cheetsheet for different tools and technologies

## Alembic
*link: https://alembic.sqlalchemy.org/en/latest/tutorial.html*

- Create migration: `alembic revision -m 'put migration's name here'`

- Apply migration: `alembic upgrade head`

- Rollback latest migration: `alembic downgrade -1`

- See current revision info: `alembic current`

- See full history of revisions: `alembic history --verbose`
