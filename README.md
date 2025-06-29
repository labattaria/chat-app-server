**Read in another language: [Українська](README.ukr.md), [English](README.md).**

# Chat app server

---

[![GraphQL](https://img.shields.io/badge/GraphQl-E10098?style=for-the-badge&logo=graphql&logoColor=white)](#)
[![JavaScript](https://img.shields.io/badge/JavaScript-323330?style=for-the-badge&logo=javascript&logoColor=F7DF1E)](#)
[![ApolloGraphQL](https://img.shields.io/badge/-ApolloGraphQL-311C87?style=for-the-badge&logo=apollo-graphql)](#)
[![SQLite](https://img.shields.io/badge/sqlite-%2307405e.svg?style=for-the-badge&logo=sqlite&logoColor=white)](#)
[![JWT](https://img.shields.io/badge/JWT-black?style=for-the-badge&logo=JSON%20web%20tokens)](#)
[![Nodemon](https://img.shields.io/badge/NODEMON-%23323330.svg?style=for-the-badge&logo=nodemon&logoColor=%BBDEAD)](#)

This is the Express/GraphQL/Apollo server, designed and configured for the **Chat Application**

This is an Express/GraphQL server with a built-in small SQLite database. It uses JSON Web Token for user authentication. Another feature is support for the WebSocket protocol, which enables bidirectional communication between the client and server through a single persistent TCP connection.

This server also uses GraphQL Subscriptions, which, together with the WebSocket protocol, allows us to receive fresh data instantly without making separate requests.

Both the client and server can send messages to each other simultaneously, making it ideal for real-time applications.

This server is only part of the application, the second part (the client) is located at this repo: [Chat client](https://github.com/labattaria/chat-app-client)

The app in this repo is deployed at [https://render.com](https://render.com), hosting public URL: [https://chat-app-server-0qdt.onrender.com/graphql](https://chat-app-server-0qdt.onrender.com/graphql)

But you can use this server manually on your local machine

## Used dependencies:

- **GraphQL** - Core GraphQL library
- **Graphql-subscriptions** – Enables implementing GraphQL subscriptions to push real-time data to clients
- **Graphql-ws** – WebSocket transport implementation for GraphQL subscriptions
- **Apollo-server** - GraphQL server that works with any GraphQL schema
- **SQLite** - A lightweight, self-contained SQL database engine. It stores the entire database in a single file
- **JWT (JSON Web Token)** - A compact, URL-safe token format used for securely transmitting information between parties. Commonly used for authentication and authorization in web applications
- **Nodemon** - A development utility that automatically restarts your Node.js server when it detects file changes

The full list of dependencies can be found in the **package.json** file.

---

## Contents

- [Installation](#installation)
- [Usage](#usage)

### Installation

1. Clone the repository:

```shell
git clone https://github.com/labattaria/chat-app-server.git
```

2. Install project dependencies:

```shell
cd chat-app-server
npm install
```

### Usage

Start the server using the following command:

```shell
npm start
```

Server will be located at **http://localhost:9000/graphql**
