# How To Run AMS Landing Page 
To access the code here is the Lnik to the repository
[AMS-Landing-Page](https://github.com/AMS-farm-management/ams-landing-page)

# Project Structure

| Folder/File                         | Description                  |
|-------------------------------------|------------------------------|
| LICENSE                             | License file                |
| package.json                        | Package configuration       |
| package-lock.json                   | Package lock file           |
| public                              | Public assets folder        |
| ├── apple-touch-icon.png            | Apple touch icon            |
| ├── favicon-192x192.png             | Favicon 192x192             |
| ├── favicon-512x512.png             | Favicon 512x512             |
| ├── favicon.ico                     | Favicon                     |
| ├── images                          | Image folder                |
| │   ├── logged_in                   | Logged-in images            |
| │   │   ├── image10.jpg             | Image 10                    |
| │   │   ├── image1.jpg              | Image 1                     |
| │   │   └── profilePicture.jpg      | Profile picture             |
| │   └── logged_out                  | Logged-out images           |
| │       ├── blogPost1.jpg           | Blog post 1                 |
| │       └── headerImage.jpg         | Header image                |
| ├── index.html                      | Main HTML file              |
| ├── js                               | JS folder                   |
| │   └── script.js                   | Main JavaScript file        |
| ├── manifest.json                   | Manifest configuration      |
| ├── robots.txt                      | Robots.txt file             |
| └── vector-file.png                 | Vector image                |
| README.md                           | Readme file                 |
| src                                 | Source code folder          |
| ├── App.js                          | Main app component          |
| ├── App.test.js                     | App test file               |
| ├── assets                           | Assets folder               |
| │   ├── images                      | Image folder                |
| │   │   └── chartaverage_1.png      | Chart image                 |
| │   ├── notification.mp3            | Notification sound          |
| │   ├── part1.png                   | Part 1 image                |
| │   ├── pricing.png                 | Pricing image               |
| │   ├── Team                        | Team images folder          |
| │   │   ├── Ansty.png               | Ansty image                 |
| │   │   └── TED.png                 | TED image                   |
| ├── Config                           | Configuration folder        |
| │   └── url.js                      | URL configuration           |
| ├── GlobalStyles.js                  | Global styles               |
| ├── index.js                        | Entry point                 |
| ├── layout                           | Layout components           |
| │   ├── AppLayout.jsx                | Layout component            |
| │   ├── Footer.jsx                   | Footer component            |
| │   ├── Header.jsx                   | Header component            |
| │   └── Sidebar.jsx                  | Sidebar component           |
| ├── logged_out                       | Logged-out components       |
| │   ├── components                   | Various components          |
| │   │   ├── About                    | About page component        |
| │   │   ├── Blog                     | Blog components             |
| │   │   ├── Dashboard                | Dashboard components        |
| │   │   ├── footer                   | Footer component            |
| │   │   ├── home                     | Home page components        |
| │   │   ├── Login                    | Login components            |
| │   │   ├── Main                     | Main page components        |
| │   │   ├── navigation               | Navigation components       |
| │   │   ├── register_login           | Register/Login pages        |
| │   │   └── Routing.js               | Routing configuration       |
| ├── Pages                            | Pages folder                |
| │   └── WeeklyReport.js              | Weekly report page          |
| ├── service-worker.js                | Service worker              |
| ├── serviceWorkerRegistration.js    | Service worker setup        |
| ├── setupTests.js                    | Test setup                  |
| ├── shared                           | Shared components           |
| │   ├── components                   | Reusable components         |
| │   └── functions                    | Utility functions           |
| ├── styles.css                       | Global styles               |
| └── theme.js                         | Theme configuration         |
| yarn.lock                            | Yarn lock file              |

# How to Run the Project

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Prerequisites

- [Node.js](https://nodejs.org/) (v14 or higher recommended)
- npm or [Yarn](https://yarnpkg.com/) for dependency management

## Steps to Run

1. **Clone the Repository**
```bash
git clone git@github.com:AMS-farm-management/ams-landing-page.git
    cd ams-landing-page
```
2. ### Install Dependencies

```bash
npm install
```
3. **Start the Development Server**
```bash
npm start or yarn start
```

---




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

     
