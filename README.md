![CircleCI](https://img.shields.io/circleci/build/github/ShipyardSuite/project/develop?label=build%20%28develop%29&logo=circleci&style=flat-square)
![CircleCI](https://img.shields.io/circleci/build/github/ShipyardSuite/project/master?label=build%20%28master%29&logo=circleci&style=flat-square)
![Docker Image Version (latest by date)](https://img.shields.io/docker/v/shipyardsuite/project?logo=docker&logoColor=ffffff&sort=date&style=flat-square)
![Codecov branch](https://img.shields.io/codecov/c/github/ShipyardSuite/project/develop?label=coverage&logo=codecov&logoColor=ffffff&style=flat-square)
![Codacy branch grade](https://img.shields.io/codacy/grade/1b323e091d9544158b5be75432136fc6/develop?label=code%20quality%20&logo=codacy&style=flat-square)
![GitHub last commit (branch)](https://img.shields.io/github/last-commit/shipyardsuite/project/develop?logo=github&style=flat-square)
![GitHub issues](https://img.shields.io/github/issues-raw/shipyardsuite/project?logo=github&style=flat-square)
![GitHub](https://img.shields.io/github/license/shipyardsuite/project?style=flat-square)

# nodejs-service-template

Project management microservice

## Environment variables

| Name                  | Type     | Default | Description                       |
| --------------------- | -------- | ------- | --------------------------------- |
| **SERVICE_NAME:**     | `String` | project | Microservice name.                |
| **SERVICE_PORT:**     | `Number` | 3007    | Microservice port.                |
| **DATABASE_URL:**     | `String` |         | Database url.                     |

## API

| Type | URL             | Body                                        | Query               | Response               | Description                                             |
| ---- | ----------------| ------------------------------------------- | -------------------- | ---------------------- | ------------------------------------------------------- |
| PUT  | `/api/update`   |                                             |                      |                        | Update user informations.                               |
| GET    | `/api/hello`       |                                        |                      | **success**: `boolean` | Testing service connection.                             |
| POST   | `/api/create`      | **creator**: `String`, **title**: `String` |                      |                        |                                                         |
| GET    | `/api/one/:id`     |                                            |                      | | |
| DELETE | `/api/delete`      |                                            |  **id**: `String`    | | |
| POST   | `/api/join`        |                                        | **projectId**: `String`, **userIdd**: `String` | | |
| GET    | `/api/all`         |                                        |                      | | |
| GET    | `/api/all/creator` |                                        | **userId**: `String` | | |
| GET    | `/api/all/team`    |                                        | **userId**: `String` | | |
| POST   | `/api/token`       | **id**: `String`                       |                      | | |
| GET    | `/api/token/:id`   |                                        |                      | | |
| UPDATE | `/api/token`       | **id**: `String`                       |                      | | |

## Usage

**LOCAL**: create a `.env` file, with the specified variables and run `docker-compose up -d --build`.

## License

This project is released under the [Apache version 2](LICENSE) license.
