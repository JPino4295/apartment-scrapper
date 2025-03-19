# Environment Variables

| Variable          | Mandatory | Description                                                                                   |
|-------------------|-----------|-----------------------------------------------------------------------------------------------|
| BASE_URL          | YES       | The base url to search. Right now only accepts Idealista                                      |
| SEARCH_URL        | YES       | The search url to search. Right now only accepts from Idealista. Must not start with /        |
| USER_AGENT        | NO        | Desired User-Agent.                                                                           |
| TELEGRAM_TOKEN    | YES       | Token of the telegram bot                                                                     |
| TELEGRAM_GROUP_ID | YES       | Id from the group where the bot will be sending messages                                      |
| DB_URL            | YES       | MongoDb url                                                                                   |
| TESTING           | NO        | true if testing, false for production. When testing, nothing related with the db will be done |

This environment variables are set by default in the docker-compose

MongoDB: Version used 4.4.6

# Pre requisites
 - Docker (https://docs.docker.com/engine/install/) or Colima (https://github.com/abiosoft/colima)
 - Docker compose (https://docs.docker.com/compose/)
 - Create a Telegram bot (https://core.telegram.org/bots/tutorial#getting-ready)

# Prepare the environment
 - Run `docker compose up -d` or `docker-compose up -d` in older versions to create the containers for the database

# Start
To iniciate the process, just use node index.js

# Notes
To use this parser in an effective way, I'd recommend to use it with an automatic starter such as cron.