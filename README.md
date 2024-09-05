# Sitemate-Full-Stack-Engineer Challange: Challenge-Q3-24

Sitemate's Full Stack Engineer Challenge Q3 24. This repository serves as a showcase of my technical skillset, abilities, demonstrating my skills and suitability for joining the Sitemate team. Please go though step by step intrsuctions for aquick code walkthrough

## OvervieIntroduction

A simple REST API Server + Client for Issues. 
Issues can be hard-coded JSON objects with just 3 attributes: id, title + description. 
The client + server should accept or send these hardcoded JSON objects according to each API call: Create, Read, Update & Delete.

In this project, Issues are represented as hard-coded JSON objects with just 3 attributes: id, title, and description. The client and server are designed to accept or send these hard-coded JSON objects according to thsese given API calls: Create, Read, Update & Delete.

## Technologies, tools and DBs Used

- JavaScript
- MongoDB
- Jest for unit testing
- ESLint
- Prettier
- dotenv for database security
- Mongoose
- ThunderClient for route configuration


## File hierarchy and Code Organization

### RESTful API Server

The server-side code is organized into the following directories within the "src" folder:

- `controllers`: Contains logic for handling requests and responses.
- `loaders`: Responsible for loading necessary configurations and initializing the application.
- `models`: Defines data models and interacts with the database.
- `tests`: Houses unit tests written using Jest.
- `validators`: Contains validation logic for incoming data.
- `routes`: Defines API endpoints and their corresponding controllers.

### REST API Client for Testing

The client-side code is organized within the `client` directory, containing the following components:

#### Services

- **Manager Service**: Handles the management of issues. It contains functions for creating, updating, and deleting issues. Additionally, it includes methods for fetching all issues or a specific issue from the server.

- **Requester Service**: Responsible for making HTTP requests to the server. It abstracts away the details of the HTTP communication, providing a cleaner interface for the manager service to interact with.

- **API Calls**: Within the services, there are functions dedicated to making specific API calls, such as `createIssue`, `updateIssue`, `getIssues`, and `deleteIssue`. These functions encapsulate the logic for communicating with the server's endpoints.

#### Main Server Functionality

- **Integration with Server API**: The client's main function is to interface with the server's API. This is achieved by calling the appropriate functions from the manager service based on user interactions or application requirements.

- **User Interface**: While not explicitly mentioned, the client likely includes user interface components responsible for displaying retrieved data and interacting with users. These components would utilize the services to perform CRUD operations on issues.

## Instructions for Running the System

To execute this project locally, follow these steps:

1. Clone the repository to your local machine
   ```bash
   git clone "myRepo Url"
   ```
2. Navigate to the project directory

3. Install project dependencies
   ```bash
   npm install
   ```
   
4. To start the backend development server, run
   ```bash
   npm start
   ```

5. To start the client-side system locally, via the terminal, input the following command
   ```bash
   \src\client\apiClientFunction.js
   ```

6. After navigating to the directory mentioned in step 5, you can execute the following command in the terminal
   ```bash
    node apiClientFunction.js
   ```

7. To run unit tests, use the following command
   ```bash
   npm test
   ```



