# Rust Search Engine

A search engine built with Rust, Actix Web, and MongoDB, deployed on DigitalOcean.

## Features
- **CRUD Operations**: Create, Read, Update, Delete operations for managing data.
- **Search Functionality**: Search through the data using MongoDB queries.
- **API Endpoints**: RESTful API endpoints for interacting with the search engine.
- **Pagination**: Pagination support for search results.
- **Authentication**: Basic authentication and authorization (if applicable).

## Technologies
- [Rust](https://www.rust-lang.org/)
- [Actix Web](https://actix.rs/)
- [MongoDB](https://www.mongodb.com/)
- [DigitalOcean](https://www.digitalocean.com/)

## Getting Started

### Prerequisites
- Rust (latest version)
- MongoDB
- Docker (for deployment)
- DigitalOcean account

### Installation
1. Clone the repository:
    ```bash
    git clone https://github.com/jayadityadev/Rust-Bootcamp.git
    ```
2. Install dependencies:
    Navigate into the directory using `cd` and build the source code
    ```bash
    cd Rust-Bootcamp
    cargo build
    ```
3. Set up MongoDB:
    * Install MongoDB and start the service.
    * Create a database and collection for your data.
    * Seed the database with initial data.

### Running the application
1. Start the MongoDB service:
    ```bash
    mongod --config /usr/local/etc/mongod.conf
    ```
2. Run the application:
    ```bash
    cargo run
    ```
3. Access the API at http://localhost:8080.

### Docker deployment
1. Build the Docker image:
    ```bash
    docker build -t rust-search-engine .
    ```
2. Run the Docker container:
    ```bash
    docker run -d -p 8080:8080 rust-search-engine
    ```

### DigitalOcean Deployment
1. Create a Droplet on DigitalOcean with Docker installed.
2. SSH into the Droplet and clone your repository.
3. Build and run the Docker container on the Droplet.

### API Documentation
* GET /search: Search the database.
* POST /items: Create a new item.
* GET /items/{id}: Get an item by ID.
* PUT /items/{id}: Update an item by ID.
* DELETE /items/{id}: Delete an item by ID.

### Contributing
Contributions are welcome! Please open an issue or submit a pull request.

### Contact
For any questions or suggestions, please contact [jayaditaydev26@outlook.com](mailto:jayadityadev26@outlook.com)