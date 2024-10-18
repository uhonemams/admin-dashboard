# Admin Dashboard for Report Management

This project is an **Admin Dashboard** designed to manage reports submitted through a **mobile application** developed using **Flutter**. The dashboard allows administrators to view, manage, and act upon reports, offering functionalities like filtering by urgency level, assigning reports to team members, and tracking report statuses. The application is built with **React** for the frontend and **Firebase** for hosting and backend services.

## Table of Contents
- [Demo](#demo)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Setup and Installation](#setup-and-installation)
- [Firebase Deployment](#firebase-deployment)
- [Usage](#usage)

## **Demo**
A live version of the application is available at: [Admin Dashboard Live Demo](https://spillaged-test.web.app/login)

## Features

- **Report Management:** View, filter, and manage reports submitted via the Flutter mobile application.
- **Status Tracking:** Change the status of reports (e.g., in progress, rejected, or completed).
- **Urgency Filtering:** Easily filter reports by urgency level for quick prioritization.
- **Employee Assignment:** Assign reports to specific team members.
- **Geolocation:** View the location of reports using Google Maps.
- **Notification System:** Pop-up notifications for successful actions like marking a report as "In Progress".
- **Responsive Design:** The dashboard is designed to work on various screen sizes.

## Tech Stack

- **Frontend:**
  - React
  - Bootstrap (for responsiveness)
  - Firebase Hosting (for deployment)
- **Backend:**
  - Firebase Firestore (for database and storage)
  
- **Mobile App (Reports Source):**
  - Developed using **Flutter**

## Setup and Installation

### Prerequisites

Before you begin, ensure you have the following installed:

- [Node.js](https://nodejs.org/) (v18.20.4 or later)
- [Firebase CLI](https://firebase.google.com/docs/cli)
- A Firebase project (set up in the [Firebase Console](https://console.firebase.google.com/))

### Steps

1. **Clone the repository:**

   ```bash
   git clone https://github.com/uhonemams/admin-dashboard.git
   ```

2. **Navigate to the project directory:**

   ```bash
   cd admin-dashboard
   ```

3. **Install dependencies:**

   ```bash
   npm install
   ```

4. **Set up Firebase:**

   Make sure you have a Firebase project set up. Run the following to configure Firebase for your project:

   ```bash
   firebase init
   ```

   Select **Hosting** and choose your Firebase project. When prompted, set the public directory to `build`.

5. **Build the project:**

   Before deploying, create a production build:

   ```bash
   npm run build
   ```

6. **Deploy to Firebase:**

   After building, deploy the app using Firebase Hosting:

   ```bash
   firebase deploy
   ```

## Firebase Deployment

The application uses Firebase Hosting for deployment. After running the `firebase deploy` command, Firebase will provide you with a hosting URL. You can access the live admin dashboard using this URL.

### Key Firebase Services Used:
- **Firebase Firestore:** Used to store reports, user data, and assignments.
- **Firebase Hosting:** Used to host the React application.

## Usage

- **Viewing Reports:** Once logged in, the dashboard displays reports submitted via the mobile app. Admins can filter reports by urgency, view report details, and assign reports to team members.
- **Assigning Reports:** Use the "Assign Report" dropdown to assign a report to a team member.
- **Changing Status:** Update the report status to "In Progress" or "Completed" using the available buttons.
- **Viewing Locations:** Click on the "View Location" link to see the report location on Google Maps.
