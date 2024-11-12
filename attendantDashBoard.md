# Attendants DashBoard  Documentation

This is a React-based web application used for managing various entities such as breeds, feeds, vaccines, farmers, and more. It provides a user interface for managing and viewing reports, schedules, and other data related to farming activities.

## Table of Contents

- [Features](#features)
- [Components](#components)
- [Services](#services)
- [Utilities](#utilities)
- [Routes](#routes)
- [Configurations](#configurations)
- [Dependencies](#dependencies)
- [Environment Variables](#environment-variables)

## Features

This application is divided into multiple features that provide interfaces for managing different aspects of the farm:

- **Home**: Dashboard for monitoring general farm data and reports.
- **Breeds**: Interface for managing animal breeds.
- **Feeds**: Interface for managing feed schedules and records.
- **Vaccines**: Interface for managing vaccine schedules and data.
- **Farmers**: Interface for managing farmers' data.
- **Settings**: Configuration options for application management.

## Components

### DashNavigation
A component that provides the navigation layout for the application.

### GeneralAnalysis
Displays general analysis data for the farm reports. 

### InDetailAnalysis
Displays detailed analysis data for the farm reports.

### OtherAnalysis
Displays other kinds of analysis data relevant to farm activities.

### PieChart
A component that renders pie charts for visualizing data insights.

### AlertsTable
Displays a table of alerts related to farm activities.

### FarmersTable
Displays a table of farmer records.

### FeedsTable
Displays a table of feed records.

### VaccinesTable
Displays a table of vaccine data.

### Steps
Displays a step-by-step guide for managing breeds or other farm activities.

## Services

Services provide the core data-fetching and API interactions:

- **HomeService**: Fetches data for the Home feature.
- **BreedService**: Fetches data for the Breeds feature.
- **FeedService**: Fetches data for the Feeds feature.
- **VaccineService**: Fetches data for the Vaccines feature.
- **FarmerService**: Fetches data for the Farmers feature.

## Utilities

These are utility hooks and functions used throughout the application:

- **ApiErrorHandler**: Handles API errors gracefully.
- **useQuery**: Custom hook for fetching data using React Query.
- **useNavigate**: Provides navigation functionality within the application.
- **useEditPassword**: Custom hook for editing passwords.
- **useVerifyEmail**: Custom hook for verifying emails.

## Routes

The application includes several routes to render different pages:

- **Home**: `/`
- **Breeds**: `/breeds`
- **Feeds**: `/feeds`
- **Vaccines**: `/vaccines`
- **Farmers**: `/farmers`
- **Settings**: `/settings`

## Configurations

- **tailwind.config.js**: Configures Tailwind CSS for utility-first styling.
- **index.html**: Configures the application's HTML structure.

## Dependencies

The application relies on the following dependencies:

- **React**: JavaScript library for building user interfaces.
- **React Router**: Library for managing navigation and routing.
- **Tailwind CSS**: Utility-first CSS framework for styling.
- **React Query**: Library for data fetching and caching.
- **React Icons**: Library for using icons within React.

## Environment Variables

The following environment variables are used in the application:

- `VITE_BASE_URL`: Base URL for the API.
- `VITE_ATTENDANT_DOMAIN`: Domain for the attendant interface.
- `VITE_ADMIN_DOMAIN`: Domain for the admin interface.
- `VITE_PUBLIC_VAPID_KEY`: Public VAPID key for notifications.
- `VITE_PRIVATE_VAPID_KEY`: Private VAPID key for notifications.


## API Endpoints

The application interacts with the following API endpoints:

- **Authentication**:
  - `POST /auth/login`: Login endpoint.
  - `POST /auth/logout`: Logout endpoint.
  - `POST /auth/verify`: Verify email.
  - `POST /auth/change-password`: Change user password.
  - `POST /auth/edit-user`: Edit user profile.

- **Farmers**:
  - `POST /farmer/registerFarmer`: Register a new farmer.
  - `GET /attendant/getFarmers`: Get a list of farmers.
  - `DELETE /farmer/deleteFarmer`: Delete a farmer.

- **Breeds**:
  - `POST /animal/breeds`: Add a new breed.
  - `GET /animal/animalTypes`: Get a list of animal types.
  - `GET /animal/breeds`: Get breeds under a specific type.
  - `PUT /animal/update-breed`: Edit breed information.

- **Feeds**:
  - `GET /feeds/get-feeds`: Get all feed data.
  - `POST /feeds/new`: Add a new feed record.
  - `PUT /feeds/update`: Edit feed record.
  - `DELETE /feeds/delete`: Delete a feed record.

- **Vaccines**:
  - `GET /vaccine/get-vaccines`: Get a list of vaccines.
  - `POST /vaccine/add`: Add a new vaccine.
  - `POST /vaccine/add-vaccine-schedule`: Add vaccine schedule.
  - `PUT /vaccine/update`: Update vaccine information.
  - `DELETE /vaccine/delete`: Delete a vaccine.

- **Reports**:
  - `GET /report/attendant-reports`: Get general reports.
  - `GET /report/farmer-reports`: Get farm-specific reports.
  - `GET /report/download-farm-report`: Download a farm report.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Feel free to reach out if you have any questions or need further clarification!


