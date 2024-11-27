# Bookshelf API Documentation

## Overview

The Bookshelf API allows users to manage a collection of books. It provides endpoints to create, read, update, and delete books from the collection.

## Base URL

```
http://localhost:8000/api
```

## Endpoints

### Get All Books

```
GET /books
```

**Response:**

```json
[
    {
        "id": 1,
        "title": "Book Title",
        "author": "Author Name",
        "published_date": "YYYY-MM-DD",
        "isbn": "ISBN Number",
        "pages": 123,
        "language": "Language",
        "publisher": "Publisher Name"
    },
    ...
]
```

### Get a Single Book

```
GET /books/{id}
```

**Response:**

```json
{
  "id": 1,
  "title": "Book Title",
  "author": "Author Name",
  "published_date": "YYYY-MM-DD",
  "isbn": "ISBN Number",
  "pages": 123,
  "language": "Language",
  "publisher": "Publisher Name"
}
```

### Create a New Book

```
POST /books
```

**Request Body:**

```json
{
  "title": "Book Title",
  "author": "Author Name",
  "published_date": "YYYY-MM-DD",
  "isbn": "ISBN Number",
  "pages": 123,
  "language": "Language",
  "publisher": "Publisher Name"
}
```

**Response:**

```json
{
  "id": 1,
  "title": "Book Title",
  "author": "Author Name",
  "published_date": "YYYY-MM-DD",
  "isbn": "ISBN Number",
  "pages": 123,
  "language": "Language",
  "publisher": "Publisher Name"
}
```

### Update a Book

```
PUT /books/{id}
```

**Request Body:**

```json
{
  "title": "Updated Book Title",
  "author": "Updated Author Name",
  "published_date": "YYYY-MM-DD",
  "isbn": "Updated ISBN Number",
  "pages": 123,
  "language": "Updated Language",
  "publisher": "Updated Publisher Name"
}
```

**Response:**

```json
{
  "id": 1,
  "title": "Updated Book Title",
  "author": "Updated Author Name",
  "published_date": "YYYY-MM-DD",
  "isbn": "Updated ISBN Number",
  "pages": 123,
  "language": "Updated Language",
  "publisher": "Updated Publisher Name"
}
```

### Delete a Book

```
DELETE /books/{id}
```

**Response:**

```json
{
  "message": "Book deleted successfully"
}
```

## Error Handling

All error responses will have the following format:

```json
{
  "error": "Error message"
}
```

## Authentication

Currently, the API does not require authentication.

## License

This project is licensed under the MIT License.
