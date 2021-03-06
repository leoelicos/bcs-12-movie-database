# Movie Database

![Node.js](https://img.shields.io/badge/16.15.0%20LTS-0?label=Node.js&style=for-the-badge&labelColor=white&color=black) ![Express.js](https://img.shields.io/badge/4.18.1-0?label=Express&style=for-the-badge&labelColor=white&color=black) ![Mysql2](https://img.shields.io/badge/2.3.3-0?label=Mysql2&style=for-the-badge&labelColor=white&color=black)

## Introduction

Moovee Database stores a database of movies.

The app uses `express.js` to coordinate the routes, and `mysql2` to handle the database;

I made this app to learn about `sql` including creating, reading, updating and deleting actions via `mysql2`.

## Installation

| Steps                        | Details                                                                                                |
| ---------------------------- | ------------------------------------------------------------------------------------------------------ |
| Install `Node.js `           | https://nodejs.org/en/                                                                                 |
| Install `Mysql`              | https://dev.mysql.com/downloads/installer/                                                             |
| Install `Insomnia`           | https://insomnia.rest/download                                                                         |
| Clone this repo              | ` git clone https://github.com/leoelicos/bcs-12-movie-database.git`                                    |
| Go inside                    | ` cd bcs-12-movie-database`                                                                            |
| Initialize and seed database | `cd db`<br>`mysql -u root -p`<br>`{password}`<br>`source schema.sql;`<br>`source seeds.sql;`<br>`exit` |
| Install dependencies         | ` npm install`                                                                                         |
| Test in Insomnia             | See [Usage](#usage)                                                                                    |

## Usage

### Insomnia

| Steps                              | Details                                                                                                       |
| ---------------------------------- | ------------------------------------------------------------------------------------------------------------- |
| Start the server from command line | `npm start`                                                                                                   |
| Root endpoint                      | GET `localhost:3001`                                                                                          |
| Search all movies                  | GET `/api/movies`                                                                                             |
| Find a specific movie              | GET `/api/movie/:id`                                                                                          |
| Search all reviews                 | GET `/api/reviews`                                                                                            |
| Find a specific review             | GET `/api/review/:id`                                                                                         |
| Add a movie                        | <p>POST `/api/add-movie`</p><p>Body: `{`</p><p>`"movie_name": STRING`</p><p>`}`</p>                           |
| Add a review                       | <p>POST `/api/add-review`</p><p>Body: `{`</p><p>`"movie_id": INTEGER,`</p><p>`"review": STRING`</p><p>`}`</p> |
| Update a movie                     | <p>PUT `/api/update-movie`</p><p>Body: `{`</p><p>`"id": INTEGER`</p><p>`"movie_name": STRING`</p><p>`}`</p>   |
| Update a review                    | <p>PUT `/api/update-review`</p><p>Body: `{`</p><p>`"id": INTEGER`</p><p>`"review": STRING`</p><p>`}`</p>      |
| Delete a movie                     | DELETE `/api/movie/:id`                                                                                       |
| Delete a review                    | DELETE `/api/review/:id`                                                                                      |

## Video Demo

https://user-images.githubusercontent.com/99461390/170400648-e9cc2c47-8fdf-4c52-9e60-3d98ee983d24.mp4

## Screenshots

### Screenshot: Schema

![Schema](https://user-images.githubusercontent.com/99461390/170399608-cc1ef5de-a41d-4134-8a3c-12c18bdc170f.png)

### Screenshot: Insomnia testing

![Insomnia testing](https://user-images.githubusercontent.com/99461390/170399527-6e4980a4-afea-4a78-9d68-91370f6ad16e.jpg)

## Credits

-  BCS Resources

## License

&copy; Leo Wong <leoelicos@gmail.com>

Licensed under the [MIT License](./LICENSE).
