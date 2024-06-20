
## Backend Server for Windows Desktop App

This backend server is designed to work with a Windows desktop application resembling Google Forms. It is built using TypeScript and Express, with JSON file storage for form submissions.



## Features


Endpoints:


`/ping: GET request to check server status.

/submit: POST request to submit form data (parameters: name, email, phone, github_link, stopwatch_time).

/read: GET request with query parameter index (0-indexed) to retrieve form submissions.


## Getting Started

1. Clone the Repository:

```bash
 git clone <repository_url>
cd backend-server

```
2. Install Dependencies:

```bash
npm install
```

3. Run the Server:

```bash
npm start
The server will start running at `http://localhost:3000.`

```
4. Endpoints:

```bash
Ping Endpoint:

`GET http://localhost:3000/ping`
Expected response: true

Submit Endpoint:
`POST http://localhost:3000/submit`

Body:
`
{
  "name": "John Doe",
  "email": "john.doe@example.com",
  "phone": "123-456-7890",
  "github_link": "https://github.com/johndoe",
  "stopwatch_time": "00:15:30"
}`

Read Endpoint:
`GET http://localhost:3000/read?index=0`

Replace 0 with the desired index (0-indexed).

Shutdown the Server: Press Ctrl + C in the terminal to stop the server.
```







## Dependencies

 * Express: Fast, unopinionated, minimalist web framework for Node.js.

* TypeScript: Typed superset of JavaScript that compiles to plain JavaScript.
