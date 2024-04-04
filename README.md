# Lisper Project

## Overview

This project is a simple web application that displays a randomly generated secret and the associated username. The application utilizes Express.js for server-side handling and Axios for making HTTP requests. The frontend is rendered using EJS (Embedded JavaScript) templates.

## Technologies Used

* [Express.js](https://expressjs.com/) - A fast, minimalist, and unopinionated web framework for Node.js
* [Axios](https://axios-http.com/docs/intro) - A promise-based HTTP client for the browser and Node.js
* [EJS](https://ejs.co/) - An embedded JavaScript template engine for Node.js

## Setup and Installation

To run this project, you will need to have Node.js and npm (Node Package Manager) installed on your machine. Follow these steps:

1. Clone the repository to your local machine using Git:
```bash
git clone https://github.com/madnoiseless/Lisper.git
```
2. Navigate to the project directory:
```bash
cd lisper
```
3. Install the required dependencies by running:
```bash
npm install
```
4. Start the server by running:
```bash
node index.js
```
The server will run on `http://localhost:3000`. Open your browser and visit this URL to see the application in action.

## How it Works

1. The server, created using Express.js, listens for incoming requests on port 3000.
2. When a user visits the root URL, the server responds with an HTTP GET request to `https://secrets-api.appbrewery.com/random`.
3. Axios handles the HTTP request and retrieves a random secret and username from the API.
4. The server renders the EJS template "index.ejs" and passes the retrieved secret and username as variables.
5. The rendered HTML is sent back as a response to the user's browser, displaying the secret and username.

## Contributing

Contributions, issues, and feature requests are welcome! If you find any bugs or have suggestions for improvements, please submit a pull request or open an issue in the GitHub repository.
