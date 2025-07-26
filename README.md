# <img align="center" width="32" height="32" alt="icon" src="https://github.com/user-attachments/assets/aaa9c425-cb06-4fc4-8b0c-b4a2aa0d29b7" /> Leads Tracker - Web App

A simple and effective web application to save and manage your leads (URLs). This app, powered by Firebase Realtime Database, allows you to store links manually and access them from any device. It's designed to be installable as a Progressive Web App (PWA) and added to your home screen for quick access.

This project was developed as part of my journey through [Scrimba's](https://scrimba.com/home) courses, specifically on Day 49 of my [100 Days of Code](https://github.com/ankitchamke/100-days-of-code) challenge.

## Features

- 🚀 **Add Leads Manually:** Easily save URLs by typing them into the input field.
- 💾 **Cloud Storage with Firebase:** All saved leads are persisted in real-time using Firebase Realtime Database, ensuring your data is always available and synchronized across devices.
- 👁️️ **View All Saved Leads:** See all your stored leads displayed as clickable links.
- 🗑️ **Delete All Leads:** Double-click the "DELETE ALL" button to clear all saved leads from the database.
- 📱 **Installable PWA:** Add the app to your home screen for a native app-like experience on your mobile device or desktop.

## UI Preview

soon™

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

## How to Add to Home Screen (PWA)

On most modern browsers (Chrome, Edge, Safari, Firefox), you can add this web app to your home screen:

* **On Desktop:** Look for an "Install app" icon in the browser's address bar (often a monitor with a down arrow or a plus sign). Click it and follow the prompts.
* **On Mobile:**
    * **Chrome/Android:** Tap the three dots menu, then select "Add to Home screen."
    * **Safari/iOS:** Tap the Share icon (box with an arrow pointing up), then scroll down and select "Add to Home Screen."
