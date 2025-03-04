# IKARUS-3D
Project Submision for IKARUS 3D 
This is a 3D solar system simulation built with Three.js and Firebase. It allows you to create, modify, save, and load solar system configurations, including planets with customizable properties such as size, color, speed, and distance from the sun.

Features:
3D Solar system visualization using Three.js.
Firebase integration for saving and loading planet configurations.
Interactive user interface for adjusting planet properties (size, speed, distance, and color).
Add planets, modify their properties, and save your custom configuration.
Dynamically load saved configurations from Firebase.
Requirements
Web browser with WebGL support (e.g., Chrome, Firefox, Safari).
Firebase Account to save/load configurations.
Internet Connection for Firebase hosting.
Installation
1. Clone the Repository
First, clone the repository to your local machine:

bash
Copy
git clone https://github.com/your-username/solar-system-ikarus-3d.git
cd solar-system-ikarus-3d
2. Firebase Setup
Create a new Firebase project at Firebase Console.
Go to the Firebase console, create a Firestore database, and configure it for the web.
Replace the Firebase configuration in index.html with your own project's config values:
javascript
Copy
const firebaseConfig = {
    apiKey: "YOUR_API_KEY",
    authDomain: "YOUR_PROJECT_ID.firebaseapp.com",
    projectId: "YOUR_PROJECT_ID",
    storageBucket: "YOUR_PROJECT_ID.appspot.com",
    messagingSenderId: "YOUR_MESSAGING_SENDER_ID",
    appId: "YOUR_APP_ID",
    measurementId: "YOUR_MEASUREMENT_ID"
};
3. Open the Project
Open index.html in your browser.
Usage
Save Configuration:
Click the Save Configuration button.
Enter a name for the configuration in the prompt.
Your solar system configuration will be saved in Firebase and listed in the dropdown.
Load Configuration:
Select a configuration from the dropdown.
The system will load the selected configuration with saved planet properties.
Controls
Orbit Controls: You can interact with the solar system by dragging the mouse to rotate, zoom in, and zoom out using the mouse or trackpad.
Planet Customization: You can adjust each planet's properties (size, color, speed, distance) using the GUI provided.
Save/Load Configuration: You can save the current configuration to Firebase or load an existing one from the Firebase database.
Dependencies
This project relies on the following libraries:

Three.js: A 3D JavaScript library used to render the solar system in 3D space.
Firebase: Backend platform used to save and load configurations.
Dat.GUI: A lightweight GUI for modifying parameters in real-time.
