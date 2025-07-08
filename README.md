JustiChat – Your AI-Powered Legal Assistant
JustiChat is a simple web application designed to provide informational assistance on legal queries using the Google Gemini API. It features a clean, responsive chat interface and a secure Node.js backend to handle API interactions.

Disclaimer: This tool is for informational purposes only and does not constitute legal advice.

Features
AI-Powered Responses: Utilizes the Google Gemini API to answer legal questions.

Secure API Key Handling: Backend server proxies requests to the Gemini API, keeping your API key secure.

Responsive Design: Built with Tailwind CSS for optimal viewing on various devices.

User-Friendly Interface: Intuitive chat layout with user and bot message differentiation.

Loading Indicator: Provides feedback while the AI is processing your query.

Project Structure
justichat-app/
├── backend/
│   ├── server.js
│   ├── gemini.env
│   ├── package.json
│   ├── package-lock.json
│   └── node_modules/ (created upon npm install)
├── frontend/
│   └── index.html
├── .gitignore
└── README.md

Setup Instructions
Follow these steps to get JustiChat up and running on your local machine.

Prerequisites
Node.js (LTS version recommended) installed on your system. You can download it from nodejs.org.

npm (Node Package Manager) - comes with Node.js.

A Google Gemini API Key. You can obtain one from the Google AI Studio.

Step 1: Clone or Download the Repository
If you're using Git, clone the repository:

git clone <your-repository-url>
cd justichat-app

If you're downloading, ensure the justichat-app folder contains the backend and frontend subdirectories as described in the "Project Structure" section above.

Step 2: Configure the Backend
Navigate to the backend directory:

cd backend

Create a .env file:

In the backend directory, create a new file named gemini.env.

Open gemini.env and add your Gemini API key:

GEMINI_API_KEY=YOUR_GEMINI_API_KEY_HERE

Replace YOUR_GEMINI_API_KEY_HERE with your actual API key.

Install Node.js dependencies:

While still in the backend directory, run the following commands:

npm init -y
npm install express cors axios dotenv body-parser

This will create package.json, package-lock.json, and the node_modules folder inside your backend directory.

Start the Backend Server:

In the same backend directory, run:

node server.js

You should see ✅ Server running at http://localhost:3000. Keep this terminal window open; the server must be running for the frontend to work.

Step 3: Launch the Frontend
Navigate to the frontend directory in your file explorer:

Go to justichat-app/frontend/

Open index.html:

Double-click on the index.html file. It will open in your default web browser.

You can now start interacting with JustiChat!

Usage
Type your legal query into the input field at the bottom of the chat window.

Press Enter or click the "Send" button.

JustiChat will display "Thinking..." while it processes your request.

The AI's response will appear in the chat window.

Technologies Used
Frontend: HTML, CSS (Tailwind CSS), JavaScript

Backend: Node.js, Express.js

API: Google Gemini API

Libraries: axios, cors, dotenv, body-parser

Contributing
Feel free to fork this repository, submit pull requests, or open issues for any bugs or feature requests.

License
This project is licensed under the ISC License.
