# User Table
-  first name (string)
- last name (string)
- date of birth (datetime)
- username (string)
- password (string)
- short bio (string)

# Posts Table
- text (string)
- date posted (datetime)
- number of likes (integer)

# Friends
- requestor user id (string)
- requested user id (string)
- date requested (datetime)
- status (boolean)

# Making a migration
npx knex migrate:make friends
npx knex migrate:rollback
npx knex migrate:latest

seeding = filling our db with sample test data

npx knex seed:make SEED_NAME - make seed file
npx knex seed:run - runs all seed files
