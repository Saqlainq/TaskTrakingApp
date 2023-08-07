# Task Tracker API

Welcome to the Task Tracker API! This API is a production-quality RESTful service for a task tracking application using Java and MySQL as the backend store. The API allows users to manage tasks with CRUD (Create, Read, Update, Delete) operations, and it incorporates comprehensive error handling, data validation, and logging.

## Setting up the Database

To set up the database for the Task Tracker API, follow these steps:

1. Create a MySQL database named `task_tracking_app`.
2. Create a user with appropriate privileges to access the `task_tracking_app` database. Note down the username and password for this user.
3. Set the database configuration in the `application.properties` file located in the `src/main/resources` directory. Replace the placeholders `your_database_username` and `your_database_password` with the actual username and password for the MySQL user.

## Building

To build the Task Tracker API, follow these steps:

1. Clone the repository by running `git clone https://github.com/saqlainq/task-tracker-api.git` in the terminal.
2. Navigate to the project directory using `cd task-tracker-api`.
3. Build the project using Maven by running `mvn clean install`.

## Testing

To run the tests for the Task Tracker API, execute the following commands:

1. Run unit tests: `mvn test`
2. Run integration tests: `mvn integration-test`

## Running the API

To run the Task Tracker API, execute the following command: `mvn spring-boot:run`. The API will be accessible at `http://localhost:8080`.

### API Endpoints

The API provides the following endpoints:

#### Create a new task

- Method: POST
- Endpoint: `/tasks`
- Request Body: JSON data containing the title, description, and due date of the task.

#### Retrieve a task by ID

- Method: GET
- Endpoint: `/tasks/{id}`

#### Retrieve a list of all tasks

- Method: GET
- Endpoint: `/tasks`

#### Update an existing task by ID

- Method: PUT
- Endpoint: `/tasks/{id}`
- Request Body: JSON data containing the updated title, description, and due date of the task.

#### Delete a task by ID

- Method: DELETE
- Endpoint: `/tasks/{id}`

**Contributing**

Contributions are welcome! If you find any issues or have suggestions for improvements, please open an issue or create a pull request.

