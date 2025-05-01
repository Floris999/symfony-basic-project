# StartShop API

This project is a Symfony-based application designed to explore the fundamentals of Symfony development. It includes a simple API for managing starships, showcasing the use of controllers, routing, dependency injection, and JSON responses.

## About the Project

The **StartShop API** is a learning project created to understand and implement the core concepts of Symfony. It provides a basic RESTful API for managing starship data, including endpoints to retrieve a collection of starships or a single starship by its ID.

The project was built as part of a learning journey through the **Symfony Fundamentals** course on [SymfonyCasts](https://symfonycasts.com/). This course provided a solid foundation in Symfony development, and this project serves as a practical application of the concepts covered.

## Features

- **Symfony Framework**: Built using Symfony, a powerful PHP framework for web applications.
- **RESTful API**: Provides endpoints for fetching starship data.
- **Routing**: Demonstrates the use of Symfony's attribute-based routing.
- **Dependency Injection**: Utilizes Symfony's service container to inject dependencies like repositories.
- **JSON Responses**: Returns data in JSON format for easy integration with front-end applications or other APIs.

## Endpoints

### Get All Starships
- **URL**: `/api/starships`
- **Method**: `GET`
- **Response**: Returns a JSON array of all starships.

### Get a Single Starship
- **URL**: `/api/starships/{id}`
- **Method**: `GET`
- **Response**: Returns a JSON object of the starship with the specified ID.
- **Error Handling**: Returns a 404 error if the starship is not found.

### Workarounds
If you using Laravel herd for local hosting. Which is not recommended with Symfony apps. You have to run the following command to set tailwind watch (-w). To built Tailwind and see your styling changes
- **Command**: php bin/console tailwind:build -w