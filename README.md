# Hub Desk

**Hub Desk** is a modular application built using React and Firebase, designed to serve as a central hub for hosting multiple mini apps. The platform allows for seamless addition of new mini apps without needing to update the entire app, providing a flexible environment for future expansion.

### Features:
- **Authentication**: Users can sign up and log in using Firebase Authentication. Signup requires admin approval for additional security.
- **Mini App Hub**: After logging in, users are navigated to a landing page where they can access various mini apps.
- **Admin Dashboard**: Admins can manage user permissions, approve or reject signups, and manage access to mini apps.
- **Scalability**: Easily add new mini apps by placing them into the `/src/apps/` directory without needing to update the whole app structure.

### Tech Stack:
- **Frontend**: React.js
- **Backend**: Firebase (Authentication, Firestore, Hosting)
- **Styling**: CSS / SCSS / Styled Components (choose your preferred styling method)

### Setup Instructions:
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/YOUR_USERNAME/hub-desk.git
   cd hub-desk
   ```
   
2. **Install Dependencies**:
   Make sure you have Node.js installed. Then run:
   ```bash
   npm install
   ```

3. **Firebase Setup**:
   - Create a Firebase project at [Firebase Console](https://console.firebase.google.com/).
   - Set up Firebase Authentication and Firestore in your Firebase project.
   - Add your Firebase credentials to `firebaseConfig.ts` in the `/src` directory.
   
4. **Run the App**:
   To run the app locally, use:
   ```bash
   npm start
   ```
   This will start the development server, and you can access the app at `http://localhost:3000/`.

### Project Structure:
```
/hub-desk
 ├── /public                # Static files
 ├── /src                   # Source files
 │   ├── /apps              # Mini apps
 │   │   ├── /another-app   # Placeholder for future mini apps
 │   ├── /auth              # Authentication pages (Login, Signup)
 │   ├── /admin             # Admin dashboard and modal
 │   ├── Landing.tsx        # Main landing page after login
 │   ├── App.tsx            # Main app component
 │   ├── routes.ts          # Routing configuration
 │   ├── firebaseConfig.ts  # Firebase configuration
 ├── package.json           # Project dependencies
 ├── firebase.json          # Firebase hosting and config file
 ├── .firebaserc            # Firebase project info
 ├── README.md              # Project description
```