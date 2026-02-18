# JWT Authentication Documentation

## Table of Contents

1. [Introduction](#introduction)
2. [Prerequisites](#prerequisites)
3. [Installation](#installation)
4. [Setup Instructions](#setup-instructions)
5. [Usage](#usage)
6. [Endpoints](#endpoints)
7. [Token Management](#token-management)
8. [Conclusion](#conclusion)

---

## Introduction

JSON Web Tokens (JWT) are an open, industry standard RFC 7519 method for representing claims securely between two parties. When a user logs in, the server issues a token that can be used for future requests and authorization.

## Prerequisites

- Node.js installed on your machine.
- A compatible database (e.g., MongoDB).

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/devVaibhavT/BackendAuth.git
   cd BackendAuth
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

## Setup Instructions

1. Create a `.env` file in the root directory and add the following variables:
   ```
   JWT_SECRET=your_jwt_secret_key
   MONGO_URI=your_mongo_database_connection_string
   PORT=your_desired_port
   ```

2. Start the application:
   ```bash
   npm start
   ```

## Usage

- Use the `/login` endpoint to authenticate users and receive a token.

## Endpoints

- `POST /login`
- `GET /protected`

## Token Management

- Tokens should be sent in the `Authorization` header as follows:
  ```
  Authorization: Bearer your_jwt_token
  ```

## Conclusion

This setup provides a secure environment for user authentication using JWT. Follow these instructions closely to ensure proper configuration and security practices.