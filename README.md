# E-Commerce Back End

This is the back-end for an e-commerce website built using Express.js and Sequelize. It provides a functional API that interacts with a MySQL database. The API supports various CRUD operations for categories, products, and tags, allowing users to manage e-commerce data.

## Walkthrough Video

A walkthrough video demonstrating the functionality of the application and how it meets the acceptance criteria can be found [here](https://drive.google.com/file/d/1aVpu13kr996pWfXdL-qwneFqIBx0m8-6/view).

## User Story

As a manager at an internet retail company, I want a back end for my e-commerce website that uses the latest technologies so that my company can compete with other e-commerce companies.

## Acceptance Criteria

- The application should connect to a MySQL database using the MySQL2 and Sequelize packages.
- Sensitive data such as the MySQL username, password, and database name should be stored using environment variables with the dotenv package.
- Sequelize models should be synced to the MySQL database on server start.
- The API should provide routes for performing CRUD operations on categories, products, and tags.
- The API should return formatted JSON data for the routes that retrieve data.
- The API should allow successful creation, update, and deletion of data in the database.

## Installation

1. Clone the repository: `git clone` (https://github.com/Aiahmed01/E-commerce-ORM)
2. Install the dependencies: `npm install`
3. Set up the database by running the SQL commands in `db/schema.sql`.
4. Update the environment variables in the `.env` file with your MySQL database credentials.
5. Seed the database with test data: `npm run seed`
6. Start the server: `npm start`

## Usage

The API can be accessed at `http://localhost:3001/api`. Use an API client such as Insomnia or Postman to test the API routes.

The available routes are:

- `GET /api/categories`: Get all categories
- `GET /api/categories/:id`: Get a single category by ID
- `POST /api/categories`: Create a new category
- `PUT /api/categories/:id`: Update a category by ID
- `DELETE /api/categories/:id`: Delete a category by ID

- `GET /api/products`: Get all products
- `GET /api/products/:id`: Get a single product by ID
- `POST /api/products`: Create a new product
- `PUT /api/products/:id`: Update a product by ID
- `DELETE /api/products/:id`: Delete a product by ID

- `GET /api/tags`: Get all tags
- `GET /api/tags/:id`: Get a single tag by ID
- `POST /api/tags`: Create a new tag
- `PUT /api/tags/:id`: Update a tag by ID
- `DELETE /api/tags/:id`: Delete a tag by ID

Make sure to replace `localhost:3001` with the appropriate host and port if you deploy the application to a different environment.

## Technologies Used

- Express.js
- Sequelize
- MySQL
- dotenv

## Contributing

Contributions are welcome! If you find any issues or have suggestions for improvement, please create a new issue or submit a pull request.

## License

This project is licensed under the [MIT License](link-to-license).
