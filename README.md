# cheetsheet
Cheetsheet for different tools and technologies

## Alembic

Create migration: `alembic revision -m 'put migration's name here'`

Apply migration: `alembic upgrade head`

Rollback latest migration: `alembic downgrade -1`
