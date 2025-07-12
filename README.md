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

After deployment is complete, Firebase will give you a public URL (e.g., [`https://`](https://9000-firebase-studio-1752312375173.cluster-fdkw7vjj7bgguspe3fbbc25tra.cloudworkstations.dev/login)). You can now visit this URL to use your application live!
These snapshots of the mobile app

<img width="1869" height="938" alt="Screenshot 2025-07-12 151228" src="https://github.com/user-attachments/assets/ca7b839f-7ab8-4220-976d-ac721c9f8f62" />
<img width="1898" height="966" alt="Screenshot 2025-07-12 160406" src="https://github.com/user-attachments/assets/61993880-3e4b-4c26-801f-f93797e18cda" />
<img width="1153" height="832" alt="Screenshot 2025-07-12 152057" src="https://github.com/user-attachments/assets/f83505c0-36c4-42e0-8445-66284cef153d" />
<img width="1899" height="970" alt="Screenshot 2025-07-12 151303" src="https://github.com/user-attachments/assets/86ddb969-24d5-4ed8-a035-5b251bf3ce6f" />
<img width="1318" height="914" alt="Screenshot 2025-07-12 161737" src="https://github.com/user-attachments/assets/83a68404-3294-4675-95f3-5b50dc14d772" />
<img width="1305" height="965" alt="Screenshot 2025-07-12 161713" src="https://github.com/user-attachments/assets/af8ce6d2-0858-4108-9046-cbe60b39ce71" />
<img width="1911" height="579" alt="Screenshot 2025-07-12 161011" src="https://github.com/user-attachments/assets/dd904f0e-3bfb-4c2e-8c3b-437902c15903" />
<img width="1910" height="975" alt="Screenshot 2025-07-12 161002" src="https://github.com/user-attachments/assets/6fbca435-4366-4f61-94ef-2835c17a2ddf" />
![WhatsApp Image 2025-07-12 at 19 45 48_aefc85d8](https://github.com/user-attachments/assets/e0d438ee-0418-4cb0-a5d1-d4cc80baa3c5)
![WhatsApp Image 2025-07-12 at 19 45 48_83af56cb](https://github.com/user-attachments/assets/40a3cfd9-b396-4fa9-8950-6c98ccdb679b)
![WhatsApp Image 2025-07-12 at 20 05 29_445656c0](https://github.com/user-attachments/assets/7f9bc446-1672-4fd0-80a0-6f4a41694b20)
![WhatsApp Image 2025-07-12 at 19 45 49_649ce50b](https://github.com/user-attachments/assets/9d479821-cfe7-44ea-92fb-2b939f756ca5)
![WhatsApp Image 2025-07-12 at 19 45 48_cf9bb3aa](https://github.com/user-attachments/assets/a1baf7f2-a58b-49b3-b207-4cd5631c40d4)
