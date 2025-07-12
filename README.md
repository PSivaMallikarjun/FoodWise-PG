# FoodWise PG - Smart Meal Management

This is a Next.js application designed to help Paying Guest (PG) owners manage meal planning efficiently. It uses AI to predict meal demand and provides a dashboard for real-time analytics.

## ✨ Features

- **Role-Based Access**: Separate interfaces for PG Owners (Admins) and Residents (Users).
- **User Management**: Admins can pre-register residents before they can create an account.
- **AI Demand Prediction**: Uses historical and real-time data to predict meal counts.
- **Real-time Dashboard**: Admins can view live meal confirmations.
- **Progressive Web App (PWA)**: Installable on mobile and desktop for an app-like experience with offline capabilities.
- **Multi-language Support**: Switch between English and Hindi.
- **Dark/Light Mode**: User-selectable themes.

## 🚀 Getting Started & Deployment

To get this application running in real-time on the web, you can deploy it for free using Firebase.

### Prerequisites

1.  **Node.js**: Ensure you have Node.js installed.
2.  **Firebase Account**: Create a free account at [firebase.google.com](https://firebase.google.com/).
3.  **Firebase CLI**: Install the Firebase command-line tools globally:
    ```bash
    npm install -g firebase-tools
    ```

### Deployment Steps

1.  **Create a Firebase Project**:
    - Go to the [Firebase Console](https://console.firebase.google.com/).
    - Click "Add project" and follow the on-screen instructions.

2.  **Set Up Your Web App in Firebase**:
    - Inside your new project, go to **Project Overview** and click the Web icon (`</>`) to add a new web app.
    - Give it a nickname and register the app.
    - Firebase will provide you with a `firebaseConfig` object. **Copy these credentials.**

3.  **Configure Environment Variables**:
    - In this project, create a new file named `.env.local`.
    - Paste the credentials you copied into this file, formatting them like so:
      ```
      NEXT_PUBLIC_FIREBASE_API_KEY=
      NEXT_PUBLIC_FIREBASE_AUTH_DOMAIN=your-project-id.firebaseapp.com
      NEXT_PUBLIC_FIREBASE_PROJECT_ID=your-project-id
      NEXT_PUBLIC_FIREBASE_STORAGE_BUCKET=your-project-id.appspot.com
      NEXT_PUBLIC_FIREBASE_MESSAGING_SENDER_ID=12345...
      NEXT_PUBLIC_FIREBASE_APP_ID=1:12345...:web:...
      ```

4.  **Enable Firebase Services**:
    - In the Firebase Console, go to the **Build** section.
    - **Authentication**: Click "Get started" and enable the **Email/Password** sign-in method.
    - **Firestore Database**: Click "Create database," start in **production mode**, and choose a location.

5.  **Log in to Firebase & Deploy**:
    - Open your terminal, navigate to the project directory, and log in:
      ```bash
      firebase login
      ```
    - Associate your local project with your Firebase project:
      ```bash
      firebase use --add
      ```
      Select the project you created from the list.
    - Deploy the application:
      ```bash
      npm run deploy
      ```

After deployment is complete, Firebase will give you a public URL (e.g., `https://your-app-name.web.app`). You can now visit this URL to use your application live!
