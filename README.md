
# Backend Project Structure & Backend API

| Folder/File                      | Description                                     |
|----------------------------------|-------------------------------------------------|
| ams.sql                          | SQL dump for database initialization            |
| package.json                     | Package configuration                           |
| yarn.lock                        | Yarn lock file                                  |
| src                              | Source code folder                              |
| ├── api                          | API endpoints folder                            |
| │   ├── admin                    | Admin-related handlers, routes, and services    |
| │   │   ├── admin.handlers.js    | Request handlers for admin                     |
| │   │   ├── admin.js             | Admin main module                               |
| │   │   ├── admin.routes.js      | Admin routes configuration                      |
| │   │   ├── admin.service.js     | Business logic for admin                        |
| │   │   ├── admin.utils.js       | Utility functions for admin                     |
| │   │   ├── admin.validation.js  | Input validation for admin                      |
| │   │   └── index.js             | Entry point for admin module                    |
| │   ├── animals                  | Animal-related functionality                    |
| │   │   ├── animal.handler.js    | Animal handlers                                 |
| │   │   ├── animal.models.js     | Animal data models                              |
| │   │   ├── animal.routes.js     | Animal routes configuration                     |
| │   │   ├── animal.service.js    | Animal service logic                            |
| │   │   ├── animal.validation.js | Animal input validation                         |
| │   │   ├── index.js             | Entry point for animals module                  |
| │   │   └── notifications        | Notifications for animal weight                 |
| │   │       └── animalWeightNotification.js | Notification logic for animal weight  |
| │   ├── attendant                | Attendant-related handlers and routes           |
| │   ├── auth                     | Authentication logic                            |
| │   ├── Farmer                   | Farmer module                                   |
| │   ├── feeds                    | Feeds management module                         |
| │   ├── notificationtest         | Testing notifications                           |
| │   ├── reports                  | Reports management                              |
| │   └── vaccine                  | Vaccine-related functionality                   |
| ├── config                       | Configuration files                             |
| │   ├── application.js           | Application configuration                       |
| │   ├── database.js              | Database configuration                          |
| │   ├── express.js               | Express.js setup                                |
| │   ├── logger.js                | Logger setup                                    |
| │   ├── passport.js              | Passport.js setup for authentication            |
| │   ├── queues                   | Queue management                                |
| │   ├── redis.js                 | Redis configuration                             |
| │   ├── routes.js                | API route definitions                           |
| │   └── superAdmin.js            | Super admin configuration                       |
| ├── constants                    | Constants and localization                      |
| │   ├── index.js                 | Constants definition                            |
| │   └── locale                   | Localization files                              |
| ├── cron-jobs                    | Scheduled jobs                                  |
| │   └── crons.js                 | Cron job definitions                            |
| ├── index.js                     | Entry point for the backend application         |
| ├── middleware                   | Middleware functions                            |
| │   ├── apiErrorHandler.js       | API error handling middleware                   |
| │   ├── authentication.js        | Authentication middleware                       |
| │   ├── checkRole.js             | Role checking middleware                        |
| │   ├── joiErrorHandler.js       | Joi validation error handler                    |
| │   └── rateLimiter.js           | API rate limiter                                |
| ├── utils                        | Utility functions                               |
| │   ├── apiResponse.js           | Standardized API response                       |
| │   ├── emailSender.js           | Email sending utility                           |
| │   ├── executeQuery.js          | Database query executor                         |
| │   ├── getUserSubscription.js   | Fetch user subscription details                 |
| │   └── index.js                 | Utility index                                   |
| └── workers                      | Queue workers                                   |
|     ├── notificationQueueWorker.js | Worker for notification queue                  |
|     └── reportQueueWorker.js     | Worker for report queue                         |

# How to Run the Backend Project

## Prerequisites

- [Node.js](https://nodejs.org/) (v14 or higher recommended)
- npm or [Yarn](https://yarnpkg.com/) for dependency management
- [MySQL](https://www.mysql.com/) for database setup
- [Redis](https://redis.io/) for queue management

  # Environment Variables

Create a `.env` file in the root of your project and add the following environment variables:

```env
NODE_ENV="development"
PORT=5000

EMAIL_USR="your_email@example.com"
EMAIL_PASS="your_email_password"

DB_SERVER="your_database_server"
DB_NAME="your_database_name"
DB_PASSWORD="your_database_password"
DB_USER="your_database_user"
DB_PORT="your_database_port"

JWT_SECRET="your_jwt_secret"
JWT_AUDIENCE="http://localhost:5000/"
JWT_ISSUER="http://localhost:5000/"

REDIS_PORT="your_redis_port"
REDIS_HOST="your_redis_host"

# Webpush configurations
PUBLIC_VAPID_KEY="your_public_vapid_key"
PRIVATE_VAPID_KEY="your_private_vapid_key"
```

# Post Man Api
To access the postman APIS you can access the puplished version [AMS PostMan Api](https://documenter.getpostman.com/view/31332147/2sAY52eL9a)

## Steps to Run

### Install Dependencies

```bash
npm install

     
