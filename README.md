
---

# AMS BAckend

## Overview
This is a backend API built with Node.js and Express for **AMS Livestock** used to manage livestock in the farm


## Table of Contents
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Environment Variables](#environment-variables)
- [Usage](#usage)
- [API Documentation](#api-documentation)
- [Testing](#testing)
- [Deployment](#deployment)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)

## Prerequisites
- **Node.js** v18+
- **yarn** (to install dependencies)
- **MySQL** (database)

## Installation

1. **Clone the Repository**
    ```bash
    git clone https://github.com/AMS-farm-management/ams-backend
    cd ams-backend
    ```

2. **Install Dependencies**
    ```bash
    yarn install
    ```

3. **Set Up Environment Variables**  
   Create `.env` and update with below configuration:
 

## Environment Variables
This project uses environment variables defined in a `.env` file:
| Variable           | Description                          |
|--------------------|--------------------------------------|
| `PORT`             | Port where the server will run       |
| `DATABASE_URL`     | URL of the database instance         |
| `JWT_SECRET`       | Secret key for JWT authentication    |
| `PUBLIC_VAPID_KEY` | For webpush                          |
| `DB_PASSWORD`     | password for the db user       |
| `DB_NAME`       | the db name (should be ams)    |
| `DB_SERVER` | ip address where server is running                        |
| `DB_USER`             | the database user       |
| `DB_PORT`     | port where db is running         |
| `JWT_SECRET`       | Secret key for JWT authentication    |
| `JWT_AUDIENCE` | the audience url for jwt tokens                        |
| `EMAIL_PASS`     |  for nodemailer auth       |
| `EMAIL_USR`       | for nodemailer    |
| `NODE_ENV` | Environemnt to run on                        |

## Usage

To start the development server:

```bash
yarn develop
```

The server will run at `http://localhost:3000` by default (or the port specified in the `.env` file).

### Common Commands

- **`yarn start`** - Runs the server in production mode.
- **`yarn develop`** - Runs the server with live-reloading for development.
- **`npm run format`** - Runs prettier for code formatting checks.
- **`npm test`** - Runs tests for the application. (currently not tests have been specifierd)

## API Documentation

The API follows REST conventions.

- For detailed API documentation, refer to the [API Documentation](https://documenter.getpostman.com/view/31332147/2sAY52eL9a)


---
