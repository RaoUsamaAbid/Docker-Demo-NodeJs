# Node.js REST API with MongoDB

This is a simple Node.js REST API for managing products, using MongoDB as the database. The application is Dockerized for easy development and deployment.

## Prerequisites

- [Docker](https://www.docker.com/products/docker-desktop) installed on your machine.

## Getting Started

1. Clone this repository to your local machine:

    ```bash
    git clone https://github.com/your-username/docker-demo-nodejs.git
    cd docker-demo-nodejs
    ```

2. Create a `.env` file in the project root and configure your MongoDB connection:

    ```env
    MONGODB_URI=mongodb://mongo:27017/productsdb
    PORT=3000
    ```

   - `MONGODB_URI`: MongoDB connection URL, where `mongo` is the name of the MongoDB container.
   - `PORT`: Port on which the Node.js server will run.

3. Build the Docker image:

    ```bash
    docker-compose build
    ```

4. Run the Docker containers:

    ```bash
    docker-compose up
    ```

5. Access the API at [http://localhost:3000/products](http://localhost:3000/products).

## API Endpoints

- **GET /products**: Get all products.
- **GET /products/:id**: Get a specific product by ID.
- **POST /products**: Create a new product.
- **PUT /products/:id**: Update a product by 
