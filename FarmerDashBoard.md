# AMS Farmer DashBoard Documentation

The Ams Farmer DashBoard was unique created to Monitor Farmers and their Animals in a Single Dashboard

The Dashboard is divided into two parts
1. General Farm Dashboard 
2. Single Animal Dashboard

## General Farm Dashboard

# FarmerDash Feature Documentation

The **FarmerDash** is a comprehensive and complex component that serves as a dashboard for farmers, allowing them to efficiently manage farms, paths, and homes. This feature is built using various **React components**, **services**, **hooks**, **context**, and **APIs**, providing a seamless and user-friendly experience.

---

## Components Overview

### Farm Feature Components

1. **Farm.js**
   - **Purpose**: Main component for managing farms.
   - **Functionality**: Renders a list of farms and provides options to add, edit, and delete farms.

2. **FarmList.js**
   - **Purpose**: Renders a paginated and filterable list of farms.
   - **Functionality**: Allows users to browse and filter farms easily.

3. **FarmForm.js**
   - **Purpose**: Form component for adding or editing farm details.
   - **Functionality**: Handles form submission and validation.

### Path Feature Components

1. **Path.js**
   - **Purpose**: Main component for managing paths.
   - **Functionality**: Renders a list of paths and provides options to add, edit, and delete paths.

2. **PathList.js**
   - **Purpose**: Renders a paginated and filterable list of paths.
   - **Functionality**: Allows users to browse and filter paths easily.

3. **PathForm.js**
   - **Purpose**: Form component for adding or editing path details.
   - **Functionality**: Handles form submission and validation.

### Home Feature Components

1. **Home.js**
   - **Purpose**: Main component for managing homes.
   - **Functionality**: Renders a list of homes and provides options to add, edit, and delete homes.

2. **HomeList.js**
   - **Purpose**: Renders a paginated and filterable list of homes.
   - **Functionality**: Allows users to browse and filter homes easily.

3. **HomeForm.js**
   - **Purpose**: Form component for adding or editing home details.
   - **Functionality**: Handles form submission and validation.

### Home Analytics and Reporting

1. **HomeAnalytics.js**
   - **Purpose**: Provides analytical data for homes.
   - **Functionality**: Displays charts and metrics related to home performance.

2. **HomeReports.js**
   - **Purpose**: Generates and displays reports for home data.
   - **Functionality**: Enables report generation and export options.

### Farms Feature Components

1. **Farms.js**
   - **Purpose**: Main component for managing farms (alternate to `Farm.js`).
   - **Functionality**: Renders a list of farms with options to add, edit, and delete.

2. **FarmsList.js**
   - **Purpose**: Renders a paginated and filterable list of farms.
   - **Functionality**: Similar to `FarmList.js` but optimized for large datasets.

3. **FarmsForm.js**
   - **Purpose**: Form component for adding or editing farms.
   - **Functionality**: Ensures data validation and seamless user interaction.

---

## Services Overview

1. **farmService.js**
   - **Purpose**: Provides API calls for farm management.
   - **Functionality**: Fetches, adds, updates, and deletes farm data.

2. **pathService.js**
   - **Purpose**: Provides API calls for path management.
   - **Functionality**: Handles CRUD operations for path data.

3. **homeService.js**
   - **Purpose**: Provides API calls for home management.
   - **Functionality**: Manages fetching, adding, editing, and deleting home data.

---

## Custom Hooks

1. **useFarm.js**
   - **Purpose**: Custom hook for managing farm data.
   - **Functionality**: Fetches and updates farm data, providing efficient state management.

2. **usePath.js**
   - **Purpose**: Custom hook for managing path data.
   - **Functionality**: Fetches and updates path data seamlessly.

3. **useHome.js**
   - **Purpose**: Custom hook for managing home data.
   - **Functionality**: Handles fetching, adding, and updating home data.

---

## Context Overview

1. **FarmContext.js**
   - **Purpose**: Provides a context for sharing farm data across components.
   - **Functionality**: Simplifies state management and data access.

2. **PathContext.js**
   - **Purpose**: Provides a context for sharing path data.
   - **Functionality**: Ensures consistent data flow for path-related components.

3. **HomeContext.js**
   - **Purpose**: Provides a context for sharing home data.
   - **Functionality**: Facilitates easy access to home data across the application.

---

## API Overview

1. **farmAPI.js**
   - **Purpose**: Contains endpoints for interacting with farm data.
   - **Functionality**: Manages CRUD operations for farms via RESTful APIs.

2. **pathAPI.js**
   - **Purpose**: Contains endpoints for interacting with path data.
   - **Functionality**: Facilitates API communication for path data.

3. **homeAPI.js**
   - **Purpose**: Contains endpoints for interacting with home data.
   - **Functionality**: Handles requests for fetching, updating, and managing home data.

---

## Database Models

1. **farmModel.js**
   - **Purpose**: Defines the schema and model for farm data.
   - **Functionality**: Interacts with the database to manage farm records.

2. **pathModel.js**
   - **Purpose**: Defines the schema and model for path data.
   - **Functionality**: Ensures proper data structure for paths in the database.

3. **homeModel.js**
   - **Purpose**: Defines the schema and model for home data.
   - **Functionality**: Manages home records and database interactions.

---

## How It Works

1. **User Navigation**: The user accesses the **FarmerDash** dashboard.
2. **Farm Management**: The `Farm` component fetches and displays a list of farms from the `farmService`. Users can add, edit, or delete farms using the `FarmForm` component.
3. **Path Management**: The `Path` component handles fetching paths from `pathService`, rendering them in a list, and managing CRUD operations.
4. **Home Management**: The `Home` component fetches home data from `homeService` and provides full CRUD functionality. The `HomeAnalytics` and `HomeReports` components add analytical and reporting features.
5. **Context & Hooks**: Contexts (e.g., `FarmContext`, `PathContext`, `HomeContext`) and custom hooks (e.g., `useFarm`, `usePath`, `useHome`) streamline data sharing and state management.

---



# Animal DashBoard Documentation
# AnimalDash Feature Documentation

The **AnimalDash** feature is an extensive component that offers a comprehensive dashboard for managing animals, reports, and farms. It leverages multiple **React components**, **services**, **hooks**, **contexts**, and **APIs** to deliver a seamless user experience.

---

## Overview

The **AnimalDash** feature is structured into several sub-features, each with dedicated components to handle distinct functionalities such as viewing and managing animals, generating and accessing reports, and overseeing farm data. Each sub-feature ensures efficient state management and clean data flow throughout the application.

---

## Components Overview

### AnimalDash Main Components

1. **AnimalDash.js**
   - **Purpose**: Main component for the AnimalDash feature.
   - **Functionality**: Renders the main dashboard with navigation links to Reports, Animals, and Farms.

2. **AnimalDashHeader.js**
   - **Purpose**: Renders the header section for the AnimalDash dashboard.
   - **Functionality**: Provides navigation and branding.

3. **AnimalDashFooter.js**
   - **Purpose**: Renders the footer section for the AnimalDash dashboard.
   - **Functionality**: Contains additional links and information.

---

## Reports Feature Components

### Components

1. **Reports.js**
   - **Purpose**: Main component for managing reports.
   - **Functionality**: Renders a list of reports with options to add, edit, and delete.

2. **ReportsList.js**
   - **Purpose**: Displays a paginated and filterable list of reports.
   - **Functionality**: Handles user interactions like search and pagination.

3. **ReportsForm.js**
   - **Purpose**: Provides a form for adding or editing report details.
   - **Functionality**: Manages form input and data submission.

### Services

1. **reportsService.js**
   - **Purpose**: Handles API requests for fetching, creating, updating, and deleting reports.
   - **Functionality**: Communicates with the backend to manage report data.

2. **reportModel.js**
   - **Purpose**: Defines the schema and methods to interact with the report database.
   - **Functionality**: Ensures consistent data management.

### Components (Additional)

1. **ReportCard.js**
   - **Purpose**: Renders a single report card with summary details.
   - **Functionality**: Supports quick viewing and interactions.

2. **ReportList.js**
   - **Purpose**: Renders a collection of report cards.
   - **Functionality**: Provides additional filtering and sorting options.

### Pages

1. **ReportsPage.js**
   - **Purpose**: Main page for displaying all reports.
   - **Functionality**: Combines the list and form components for a complete interface.

2. **ReportDetailPage.js**
   - **Purpose**: Displays detailed information about a single report.
   - **Functionality**: Allows editing and reviewing report specifics.

---

## Animal Feature Components

### Components

1. **Animal.js**
   - **Purpose**: Main component for managing animals.
   - **Functionality**: Renders a list of animals with options to add, edit, and delete.

2. **AnimalList.js**
   - **Purpose**: Renders a paginated list of animals.
   - **Functionality**: Supports filtering and search features.

3. **AnimalForm.js**
   - **Purpose**: Form component for adding or editing animal data.
   - **Functionality**: Validates user input and handles submission.

### Components (Additional)

1. **AnimalCard.js**
   - **Purpose**: Renders a single animal card with key details.
   - **Functionality**: Provides options for quick actions like editing or deleting.

2. **AnimalList.js**
   - **Purpose**: Displays a list of animal cards.
   - **Functionality**: Includes pagination and search features.

### Pages

1. **AnimalPage.js**
   - **Purpose**: Main page for viewing and managing animals.
   - **Functionality**: Combines list and form components for ease of use.

2. **AnimalDetailPage.js**
   - **Purpose**: Displays detailed information about a specific animal.
   - **Functionality**: Provides options to update or analyze animal data.

---

## Farm Feature Components

### Components

1. **Farm.js**
   - **Purpose**: Main component for managing farms.
   - **Functionality**: Renders a list of farms with options to add, edit, and delete.

2. **FarmList.js**
   - **Purpose**: Renders a list of farms with pagination and filtering.
   - **Functionality**: Enhances user interaction with search and sort features.

3. **FarmForm.js**
   - **Purpose**: Provides a form for adding or editing farm details.
   - **Functionality**: Handles form submission and validation.

### Components (Additional)

1. **FarmCard.js**
   - **Purpose**: Renders a single farm card with essential information.
   - **Functionality**: Supports interactions like viewing or editing farm details.

2. **FarmList.js**
   - **Purpose**: Displays a collection of farm cards.
   - **Functionality**: Enables advanced filtering and sorting.

### Pages

1. **FarmPage.js**
   - **Purpose**: Main page for managing farm data.
   - **Functionality**: Integrates list and form components.

2. **FarmDetailPage.js**
   - **Purpose**: Displays detailed information about a specific farm.
   - **Functionality**: Allows editing and provides an overview of farm data.

---

## Home Feature Components

1. **Home.js**
   - **Purpose**: Main component for the AnimalDash home feature.
   - **Functionality**: Provides navigation links to Reports, Animals, and Farms.

2. **HomeHeader.js**
   - **Purpose**: Renders the header for the home dashboard.
   - **Functionality**: Includes branding and main navigation.

3. **HomeFooter.js**
   - **Purpose**: Renders the footer for the home dashboard.
   - **Functionality**: Displays additional information and links.

---

## Services Overview

1. **animalService.js**
   - **Purpose**: API calls for managing animal data.
   - **Functionality**: Handles CRUD operations for animals.

2. **farmService.js**
   - **Purpose**: API calls for managing farm data.
   - **Functionality**: Facilitates CRUD operations for farm records.

3. **reportService.js**
   - **Purpose**: API calls for managing reports.
   - **Functionality**: Manages report data with CRUD operations.

---

## Custom Hooks

1. **useAnimal.js**
   - **Purpose**: Fetches and updates animal data.
   - **Functionality**: Simplifies data management for animal-related components.

2. **useFarm.js**
   - **Purpose**: Fetches and updates farm data.
   - **Functionality**: Provides easy data access for farm components.

3. **useReport.js**
   - **Purpose**: Fetches and updates report data.
   - **Functionality**: Optimizes data fetching for reports.

---



## API Overview

1. **animalAPI.js**
   - **Purpose**: Endpoints for animal-related data.
   - **Functionality**: Manages API interactions for animal features.

2. **farmAPI.js**
   - **Purpose**: Endpoints for farm-related data.
   - **Functionality**: Handles API requests for farms.

3. **reportAPI.js**
   - **Purpose**: Endpoints for report-related data.
   - **Functionality**: Supports CRUD operations for reports.

---

## How It Works

1. **User Interaction**: Users navigate through the **AnimalDash** dashboard, selecting either Animals, Reports, or Farms.
2. **Data Fetching**: Custom hooks (`useAnimal`, `useFarm`, `useReport`) are used to fetch and manage data efficiently.
3. **CRUD Operations**: Users can add, edit, or delete entities. Form components (`AnimalForm`, `FarmForm`, `ReportsForm`) handle input validation and data submission.
4. **State Management**: Contexts (`AnimalContext`, `FarmContext`, `ReportContext`) ensure consistent data flow and state management across components.
5. **Pages and Navigation**: Pages like `AnimalPage`, `FarmPage`, and `ReportsPage` organize features into cohesive, user-friendly layouts.

---

# API Endpoints Documentation

This document provides a comprehensive list of the available API endpoints in the **AnimalDash** feature, along with brief descriptions of each.

---

## Authentication Endpoints

1. **Login Path**
   - **Endpoint**: `/auth/login`
   - **Description**: Endpoint used for user authentication and logging in.

2. **Edit User Profile**
   - **Endpoint**: `/auth/edit-user`
   - **Description**: Allows users to update their profile information.

3. **Change Password**
   - **Endpoint**: `/auth/change-password`
   - **Description**: Allows users to change their password.

4. **Logout**
   - **Endpoint**: `/auth/logout`
   - **Description**: Logs the user out of the system.

5. **Get Profile**
   - **Endpoint**: `/auth/profile`
   - **Description**: Retrieves the logged-in user's profile information.

6. **Change Email**
   - **Endpoint**: `/auth/change-email`
   - **Description**: Updates the user's email address.

7. **Verify Email**
   - **Endpoint**: `/auth/verify`
   - **Description**: Verifies the user's email address.

8. **Request Account**
   - **Endpoint**: `/auth/request-account`
   - **Description**: Requests the creation of a new user account.

---

## Farm Management Endpoints

1. **Register Farm**
   - **Endpoint**: `/farmer/registerFarm`
   - **Description**: Registers a new farm in the system.

2. **Get Farms**
   - **Endpoint**: `/farmer/getFarms`
   - **Description**: Fetches a list of all registered farms.

3. **Get Farm Types**
   - **Endpoint**: `/farmer/getFarmTypes`
   - **Description**: Retrieves available types of farms.

4. **Edit Farm**
   - **Endpoint**: `/farmer/editFarm`
   - **Description**: Edits the details of an existing farm.

5. **Edit Farm Types**
   - **Endpoint**: `/farmer/editHouseType`
   - **Description**: Updates the types of houses or farm categories.

6. **Add House Type**
   - **Endpoint**: `/farmer/addHouseType`
   - **Description**: Adds a new type of house or farm category.

---

## Animal Management Endpoints

1. **Generate Animal Schedule**
   - **Endpoint**: `/animal/generateSchedule`
   - **Description**: Generates a feeding or management schedule for animals.

2. **Get Sick Animals**
   - **Endpoint**: `/report/sick-animals`
   - **Description**: Fetches a list of animals that are reported as sick.

3. **Get Animals That Need Vaccines**
   - **Endpoint**: `/report/vaccine-needed`
   - **Description**: Retrieves animals that are due for vaccination.

4. **Get Animal Feed Schedule**
   - **Endpoint**: `/feeds/breed-feed-schedule`
   - **Description**: Fetches the feed schedule for specific animal breeds.

5. **Get Animals Sold**
   - **Endpoint**: `/report/sold-animal-report`
   - **Description**: Provides a report on animals that have been sold.

---

## Report Endpoints

1. **Generate Farm Report**
   - **Endpoint**: `/attendant/generateHouseTypeReport`
   - **Description**: Generates a report for the farm's house types.

2. **Download Report**
   - **Endpoint**: `/report/download-farm-report`
   - **Description**: Allows users to download a generated farm report.

3. **Get Weight Report**
   - **Endpoint**: `/report/get-weight-reports`
   - **Description**: Retrieves reports detailing the weight metrics of animals.

4. **Get Monthly Feeding Cost**
   - **Endpoint**: `/report/get-monthly-feed-cost`
   - **Description**: Provides a breakdown of monthly feeding costs.

5. **Get Monthly Vaccine Cost**
   - **Endpoint**: `/report/vaccine-cost-reports`
   - **Description**: Fetches reports on the monthly cost of vaccinations.

6. **Get Farm Dashboard Report**
   - **Endpoint**: `/report/farmer-reports`
   - **Description**: Retrieves a summary report for the farm dashboard.

7. **Get Farm Monthly Feed Report**
   - **Endpoint**: `/report/farmer-monthly-feed-cost`
   - **Description**: Reports on the monthly feed cost per farm.

8. **Get Farm Monthly Mortality Report**
   - **Endpoint**: `/report/total-dead-animals`
   - **Description**: Provides a report on the total number of deceased animals monthly.

9. **Get Farm Monthly Income**
   - **Endpoint**: `/report/farm-income-reports`
   - **Description**: Summarizes the farm's monthly income.

10. **Get Farm Monthly Vaccine Report**
    - **Endpoint**: `/report/farmer-monthly-vaccine-cost`
    - **Description**: Reports the monthly vaccine costs for the farm.

11. **Get Expenditure Per Breed**
    - **Endpoint**: `/report/breed-feed-expenditure`
    - **Description**: Details the feed expenditure per animal breed.

12. **Get Breed Distribution**
    - **Endpoint**: `/report/farm-breed-report`
    - **Description**: Provides a distribution report of breeds within the farm.

13. **Notify Admin After Attendant Visits Farms**
    - **Endpoint**: `/attendant/notifyAdmin`
    - **Description**: Sends a notification to the admin after an attendant visits farms.

---

## Notifications Endpoints

1. **Get User Notifications**
   - **Endpoint**: `/report/notifications`
   - **Description**: Retrieves all notifications for the user.

2. **Mark Notification as Read**
   - **Endpoint**: `/report/mark-notification-as-read`
   - **Description**: Marks a notification as read.

---

## Miscellaneous Endpoints

1. **Edit Profile**
   - **Endpoint**: `/auth/edit-user`
   - **Description**: Edits user profile details.

2. **Request Account**
   - **Endpoint**: `/auth/request-account`
   - **Description**: Request the creation of a new account.

---

**Note**: All endpoints are relative to the `BASE_URL` defined in your environment variables.

--- 

## Example Usage

Here's how you can use these endpoints with `axios`:

```javascript
import axios from 'axios';
import { BASE_URL, GET_FARMS } from './apiEndpoints';

async function fetchFarms() {
  try {
    const response = await axios.get(`${BASE_URL}${GET_FARMS}`);
    console.log(response.data);
  } catch (error) {
    console.error("Error fetching farms:", error);
  }
}

fetchFarms();
  ```

## Setting Up the Project
```
# Base URL for the API server
VITE_BASE_URL="http://localhost:5000/api"

# URLs for different domains
VITE_ATTENDANT_DOMAIN="http://localhost:5173"
VITE_ADMIN_DOMAIN="http://localhost:5175"

# VAPID keys for Web Push Notifications
# Public VAPID Key
 - This key is safe to be shared and used for client-side push registration

VITE_PUBLIC_VAPID_KEY="Bcdtq7oZ4sAyyQYwmFCAqBtvybDxgL_rHkwHyVLIKqiDpJsVoJZ-vBvhx4"

# Private VAPID Key 
- Keep this key secure; it should never be exposed publicly

VITE_PRIVATE_VAPID_KEY="OeNOAiQLdob7B6KXVtDwq4D04MPeE9cfDA"
```


1. **Clone the repository**:
```bash
git clone <repo-url>
yarn install
yarn dev
```


