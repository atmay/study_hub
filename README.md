# cheetsheet
Cheetsheet for different tools and technologies

## Alembic

Alembic provides for the creation, management, and invocation of change management scripts for a relational database, using SQLAlchemy as the underlying engine. 

*link: https://alembic.sqlalchemy.org/en/latest/tutorial.html*

- Create migration: `alembic revision -m 'put migration's name here'`

- Apply migration: `alembic upgrade head`

- Rollback latest migration: `alembic downgrade -1`

- See current revision info: `alembic current`

- See full history of revisions: `alembic history --verbose`
