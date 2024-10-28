# CRUD API Docker Compose Example

Welcome to the **CRUD API Docker Compose Example**! This project demonstrates how to build a simple CRUD (Create, Read, Update, Delete) API using Node.js and MongoDB, all containerized with Docker and orchestrated using Docker Compose.

## 📚 Features

- **Create Items**: Add new items to the database.
- **Read Items**: Retrieve a list of all items.
- **Delete Items**: Remove items from the database.
- **Dockerized**: Run the application in isolated containers for easy deployment and management.

## 🛠 Technologies Used

- **Node.js**: For building the backend API.
- **Express**: A web framework for Node.js to handle HTTP requests.
- **MongoDB**: A NoSQL database for storing data.
- **Docker**: For containerization of the application.
- **Docker Compose**: For managing multi-container Docker applications.

## 📁 Project Structure

```
/crud-api-docker-compose
    ├── backend
    │   ├── Dockerfile         # Dockerfile for the backend service
    │   ├── package.json       # Node.js package configuration
    │   └── server.js          # Main application code
    ├── docker-compose.yml      # Docker Compose configuration
```

## 🚀 Getting Started

To set up and run this application locally, follow these steps:

### 1. Clone the repository:

```bash
git clone https://github.com/yourusername/crud-api-docker-compose.git
```

### 2. Navigate to the project directory:

```bash
cd crud-api-docker-compose
```

### 3. Build and run the application:

```bash
docker-compose up --build
```

This command will build your Docker images and start your services defined in the `docker-compose.yml` file.

### 4. Test the API

You can test your CRUD API using tools like Postman or curl:

- **Add an item**:
  ```bash
  curl -X POST http://localhost:5000/items -H "Content-Type: application/json" -d '{"name": "Item1"}'
  ```

- **Get all items**:
  ```bash
  curl http://localhost:5000/items
  ```

- **Delete an item** (replace `<id>` with the actual item ID):
  ```bash
  curl -X DELETE http://localhost:5000/items/<id>
  ```

## 🤝 Contributing

Contributions are welcome! If you have suggestions or improvements, feel free to fork the repository and submit a pull request.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

Thank you for checking out my CRUD API Docker Compose Example! Happy coding!

---

Feel free to customize any sections or add more details specific to your project!
