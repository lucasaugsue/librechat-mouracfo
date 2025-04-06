# Project Name

A brief description of your project. This project uses LibreChat, a chat system that allows parameter adjustments for customizing automated conversations. It includes local database development via Docker.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Main Commands](#main-commands)
- [Accessing the Database](#accessing-the-database)

## Installation

1. Clone the repository:

`git clone https://github.com/your-username/repository-name.git`
`cd repository-name`

Make sure Docker and Docker Compose are installed on your system.

2. Usage

Start the project: `docker compose -f ./deploy-compose.yml up -d`
Stop the project: `docker compose -f ./deploy-compose.yml down`

3. Accessing the Database

The MongoDB database is configured to run locally. To access the database, follow these steps:

Identify the container ID with the command:

`docker ps`

Access MongoDB with the command, replacing container_id with the MongoDB container ID:

`docker exec -it container_id mongosh`