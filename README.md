## Description

This is a simple movie database app that allows users to add movies to a database and view them in a list. The app is built using React and Node.js.

---

## Application Features

- Users can add movies to the database
- Users can view a list of all movies in the database
- Users can delete movies from the database
- Users can search for movies in the database
- Users can sort movies by title, genre, and year
- Users can view a list of all movies in the database

---

## Technologies Used

- React
- Node.js
- Knex.js
- Express
- PostgreSQL
- Heroku

## Backend Endpoints
### /movies
- GET: Returns a list of all movies in the database
- Request Body: None
- Response Body:
```JSON
[
    {
        "id": 1,
        "title": "The Matrix",
        "genre": "Action",
        "year": 1999
    },
    {
        "id": 2,
        "title": "The Matrix Reloaded",
        "genre": "Action",
        "year": 2003
    },
    {
        "id": 3,
        "title": "The Matrix Revolutions",
        "genre": "Action",
        "year": 2003
    }
]
```

- POST: Adds a movie to the database
- Request Body:
```JSON
{
    "title": "The Matrix",
    "genre": "Action",
    "year": 1999
}
```

- DELETE: Deletes a movie from the database

### /reviews
- GET: Returns a list of all reviews in the database
- Request Body: None
- Response Body:
```JSON
[
    {
        "id": 1,
        "movie_id": 1,
        "reviewer": "John Doe",
        "review": "This movie was great!"
    },
    {
        "id": 2,
        "movie_id": 1,
        "reviewer": "Jane Doe",
        "review": "This movie was terrible!"
    }
]
```

- POST: Adds a review to the database

- DELETE: Deletes a review from the database

### /search
- GET: Returns a list of all movies in the database that match the search query
- Request Body: None
- Response Body:
```JSON
[
    {
        "id": 1,
        "title": "The Matrix",
        "genre": "Action",
        "year": 1999
    },
    {
        "id": 2,
        "title": "The Matrix Reloaded",
        "genre": "Action",
        "year": 2003
    },
    {
        "id": 3,
        "title": "The Matrix Revolutions",
        "genre": "Action",
        "year": 2003
    }
]
```

### /sort
- GET: Returns a list of all movies in the database sorted by the specified column
- Request Body: None
- Response Body:
```JSON
[
    {
        "id": 1,
        "title": "The Matrix",
        "genre": "Action",
        "year": 1999
    },
    {
        "id": 2,
        "title": "The Matrix Reloaded",
        "genre": "Action",
        "year": 2003
    },
    {
        "id": 3,
        "title": "The Matrix Revolutions",
        "genre": "Action",
        "year": 2003
    }
]
```

### /theaters
- GET: Returns a list of all theaters in the database
- Request Body: None
- Response Body:
```JSON
[
    {
        "id": 1,
        "name": "AMC",
        "location": "New York"
    },
    {
        "id": 2,
        "name": "Regal",
        "location": "New York"
    },
    {
        "id": 3,
        "name": "AMC",
        "location": "New Jersey"
    }
]
```

- POST: Adds a theater to the database

- DELETE: Deletes a theater from the database

### /showtimes
- GET: Returns a list of all showtimes in the database
- Request Body: None
- Response Body:
```JSON
[
    {
        "id": 1,
        "movie_id": 1,
        "theater_id": 1,
        "showtime": "2021-04-20T20:00:00.000Z"
    },
    {
        "id": 2,
        "movie_id": 1,
        "theater_id": 2,
        "showtime": "2021-04-20T20:00:00.000Z"
    },
    {
        "id": 3,
        "movie_id": 2,
        "theater_id": 3,
        "showtime": "2021-04-20T20:00:00.000Z"
    }
]
```

- POST: Adds a showtime to the database

- DELETE: Deletes a showtime from the database

## Installation

To install this application, clone the repository and install dependencies using the following commands:

```
git clone
npm install
```

## Usage

To run the application locally, use the following command:

```
npm start
```
