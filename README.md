###

This is an example repo demonstrating an issue in prisma 4.1 when trying to update an index to use an expression manually.

### Steps to reproduce

- Run postgres: `docker-compose up -d postgres`
- Install dependencies: `npm i`
- Run existing migration: `npx prisma migrate deploy`
- Attempt to create migration for schema updates: `npx prisma migrate dev -name "Add last name to user"`
