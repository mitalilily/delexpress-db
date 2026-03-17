# DelExpress DB

This repo stores the PostgreSQL schema and SQL migration files for DelExpress.

Production database:
- Deploy the actual database as a managed PostgreSQL instance on Render.
- Do not deploy this repo as a web service.

How it connects:
- Create the Render Postgres database.
- Add its `DATABASE_URL` to the Render backend service.
- Run the backend migration flow against that database.
- Keep this repo as the source of truth for schema and SQL migrations.

