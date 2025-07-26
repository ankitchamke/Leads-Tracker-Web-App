# <img align="center" width="32" height="32" alt="icon" src="https://github.com/user-attachments/assets/aaa9c425-cb06-4fc4-8b0c-b4a2aa0d29b7" /> Leads Tracker - Web App

A simple and effective web application to save and manage your leads (URLs). This app, powered by Firebase Realtime Database, allows you to store links manually and access them from any device. It's designed to be installable as a Progressive Web App (PWA) and added to your home screen for quick access.

This project was developed as part of my journey through [Scrimba's](https://scrimba.com/home) courses, specifically on Day 49 of my [100 Days of Code](https://github.com/ankitchamke/100-days-of-code) challenge.

## [🔗 Live Project](https://ankitchamke-leads-tracker-web-app.netlify.app/)

You can access the live version of the Leads Tracker web app [here](https://ankitchamke-leads-tracker-web-app.netlify.app/)

⚠️ Important Note: This live demo is connected to a shared Firebase Realtime Database. This means any leads you save will be visible to, and can be modified by, anyone else accessing this link. This setup is for demonstration purposes. For a personal and private leads tracker, user authentication and data security would be implemented.

## Features

- 🚀 **Add Leads Manually:** Easily save URLs by typing them into the input field.
- 💾 **Cloud Storage with Firebase:** All saved leads are persisted in real-time using Firebase Realtime Database, ensuring your data is always available and synchronized across devices.
- 👁️️ **View All Saved Leads:** See all your stored leads displayed as clickable links.
- 🗑️ **Delete All Leads:** Double-click the "DELETE ALL" button to clear all saved leads from the database.
- 📱 **Installable PWA:** Add the app to your home screen for a native app-like experience on your mobile device or desktop.

## UI Preview

<img height = "700" src="https://github.com/user-attachments/assets/c9d3c278-c7d7-4634-8179-5a8dbaaf7550" >

## How It Works

This application utilizes vanilla JavaScript to interact with DOM elements and Firebase Realtime Database APIs. Data is stored in your Firebase project and rendered dynamically on the page.

### Main Functions:

* `render(leads)`: Renders a list of links from the `leads` array, fetching them from Firebase.
* `inputBtn`: Adds the manually entered URL to the Firebase Realtime Database.
* `deleteBtn`: Clears all saved leads from the Firebase Realtime Database on double-click.

## Technologies Used

* **HTML**
* **CSS**
* **JavaScript**
* **Firebase Realtime Database:** For real-time data storage and synchronization.

## Setup and Installation (for Developers)

To run this project locally, follow these steps:

1.  **Clone the repository:**
    ```bash
    git clone <your-repository-url>
    ```
2.  **Navigate to the project directory:**
    ```bash
    cd leads-tracker-webapp
    ```
3.  **Set up Firebase:**
    * Go to the [Firebase Console](https://console.firebase.google.com/).
    * Create a new Firebase project.
    * Enable Realtime Database for your project.
    * Copy your Firebase configuration (specifically the `databaseURL`).
    * Update the `firebaseConfig` object in your `index.js` file with your `databaseURL`:

        ```javascript
        const firebaseConfig = {
            databaseURL: "YOUR_FIREBASE_DATABASE_URL_HERE"
        }
        ```
4.  **Open `index.html` in your browser.**

## How to Add to Home Screen (PWA)

On most modern browsers (Chrome, Edge, Safari, Firefox), you can add this web app to your home screen:

* **On Desktop:** Look for an "Install app" icon in the browser's address bar (often a monitor with a down arrow or a plus sign). Click it and follow the prompts.

  <img width="700" src="https://github.com/user-attachments/assets/99115709-f712-4741-b0f2-ed3dd3b74d59" />

* **On Mobile:**
    * **Chrome/Android:** Tap the three dots menu, then select "Add to Home screen."
    * **Safari/iOS:** Tap the Share icon (box with an arrow pointing up), then scroll down and select "Add to Home Screen."

  <img width="700" src="https://github.com/user-attachments/assets/4c51a599-d6f7-42d4-9447-003c8937577e" />
