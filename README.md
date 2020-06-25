# Seeding database

To seed the database, run the psql script `psql -U dunder_mifflin -d blogful -f ./seeds/seed.blogful_articles.sql`

check dBeaver to confirm data

## Scripts for test driven development

Migrate the database at DB_URL, with `npm run migrate:test`

Migrate the tests (at TEST_DB_URL), with `npm run migrate:test`

Env setup
Remember to create a .env file with DB_URL and TEST_DB_URL.

Deploying
When your new project is ready for deployment, add a new heroku application with heroku create. This will make a new git remote called "heroku" and you can then npm run deploy which will push to this remote's master branch.
