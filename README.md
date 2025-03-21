# Medical-Consultancy-and-Healthcare-website-
This is a React-based web application that facilitates virtual medical consultations. It includes features like:

User authentication (name and phone number)
Text-based chat between users and doctors
Audio & video calling for real-time communication
Prescription management (adding & downloading prescriptions)
This is a web application and not a mobile app since it is built with React.js, optimized for browsers, and does not use any mobile-specific technologies like React Native.

Tech Stack
Frontend:
React.js – Main JavaScript library for building UI components
TypeScript – Adds static typing for better maintainability
ShadCN/UI Components – Pre-built UI components for styling
Tailwind CSS – Utility-first CSS framework for styling
Libraries & APIs Used
date-fns – Handles date and time formatting
Lucide React – Icon library used for UI elements
Browser Media API – Used for accessing audio and video streams
Features & Functionalities
1. User Authentication
Users must log in by entering their name and phone number before accessing the consultation features.

State Variables Used:

isLoggedIn → Tracks if a user has logged in
name → Stores the user's name
phoneNumber → Stores the user's phone number
How it Works:

If a user enters both fields, they can access the consultation page.
If the fields are empty, an alert is shown.
2. Chat System (User & Doctor Messages)
Users can send messages in a text-based chat, and an AI-generated doctor response is sent back.

State Variables Used:

messages → Stores chat history
inputValue → Stores the current input field value
How it Works:

User types a message and clicks Send.
Message is stored and displayed in the UI.
A simulated doctor response is added after a short delay.
Doctor Response Logic:

Predefined set of responses.
One random response is chosen and displayed.
3. Audio & Video Calling
Users can start and stop audio and video calls using browser APIs.

State Variables Used:

audioCallActive → Tracks if an audio call is active
videoCallActive → Tracks if a video call is active
audioStream → Stores the audio stream
videoStream → Stores the video stream
How it Works:

When a user starts a call, the app requests microphone/camera access.
If the user grants permission, the stream is displayed.
When the user ends the call, all active media streams are stopped.
4. Prescription Management
Users can add prescriptions and download them as text files.

State Variables Used:

prescriptions → Stores prescription details
How it Works:

Clicking "Add Prescription" generates a prescription for the logged-in user.
Prescriptions are displayed with timestamps.
Clicking "Download" saves the prescription as a .txt file.
Folder Structure
bash
Copy
Edit
/medical-consultation  
│── components/  
│   ├── ui/         # UI elements (buttons, inputs, etc.)  
│── pages/  
│   ├── MedicalConsultation.tsx  # Main file  
│── public/  
│── src/  
│── README.md  
│── package.json  

How to Run the Project:-

1. Install Dependencies
bash
Copy
Edit
npm install

2. Start the Development Server
bash
Copy
Edit
npm run dev

3. Open in Browser


