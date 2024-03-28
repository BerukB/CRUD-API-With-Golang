### README

#### Movie API

This Go program implements a simple RESTful API for managing movies. It allows users to perform basic CRUD operations (Create, Read, Update, Delete) on a collection of movies. The API is built using the Gorilla Mux router for routing HTTP requests.

#### How to Run

1. Ensure you have Go installed on your system. If not, download and install it from [Go Downloads](https://golang.org/dl/).

2. Clone this repository or copy the code into a `.go` file.

3. Open a terminal and navigate to the directory containing the main Go file.

4. Run the following command to start the server:

    ```
    go run main.go
    ```

    This will start the server locally on port 8000.

#### Endpoints

- **GET /movies**: Retrieves all movies in the collection.
- **GET /movies/{id}**: Retrieves a single movie by its ID.
- **POST /movies**: Creates a new movie.
- **PUT /movies/{id}**: Updates an existing movie by its ID.
- **DELETE /movies/{id}**: Deletes a movie by its ID.

#### Request & Response Formats

- **Request Payloads**: For POST and PUT requests, provide a JSON payload with the movie details. Example:
  
    ```json
    {
        "isbn": "1234567890",
        "title": "Sample Movie",
        "director": {
            "firstname": "John",
            "lastname": "Doe"
        }
    }
    ```

- **Response Payloads**: The API returns JSON-formatted responses for all endpoints.

#### Dependencies

- **github.com/gorilla/mux**: Gorilla Mux is used for routing HTTP requests.

#### Note

- This is a basic implementation intended for learning and demonstration purposes. Additional features such as data validation, authentication, and database integration may be needed for production use.

#### Contributors

- [Beruk Berhanu](https://github.com/BerukB)