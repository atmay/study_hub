# cheetsheet
Cheetsheet for different tools and technologies

## Cracking the coding interview highlights

- Resizing factor for Python lists depends greatly on the version of CPython but is always more than 1. For some versions it equals to 1.12. 
- Calculating complexity: 1 + 2 + .... + n equals to n(n+1)/2 or O(n^2)

## Alembic

Alembic provides for the creation, management, and invocation of change management scripts for a relational database, using SQLAlchemy as the underlying engine. 

*link: https://alembic.sqlalchemy.org/en/latest/tutorial.html*

- Create migration: `alembic revision -m 'put migration's name here'`

- Apply migration: `alembic upgrade head`

- Rollback latest migration: `alembic downgrade -1`

- See current revision info: `alembic current`

- See full history of revisions: `alembic history --verbose`
