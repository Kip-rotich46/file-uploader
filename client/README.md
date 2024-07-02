### Project Details

```markdown
# React File Upload Application

This project is a simple React application for uploading files to a server using Axios and Express.

## Table of Contents

- [Features](#features)
- [Setup Instructions](#setup-instructions)
- [Usage](#usage)
- [Technologies Used](#technologies-used)
- [Folder Structure](#folder-structure)
- [License](#license)

## Features

- Upload files via a form.
- Display upload progress with a progress bar.
- Display uploaded file details after successful upload.
- Show error messages for failed uploads.

## Setup Instructions

To run this project locally, follow these steps:

1. **Clone the repository:**

   ```bash
   git clone <repository-url>
   cd <project-folder>
   ```

2. **Install dependencies:**

   ```bash
   # Install server dependencies (assuming npm is used)
   cd server
   npm install

   # Install client dependencies
   cd ../client
   npm install
   ```

3. **Run the server and client:**

   ```bash
   # Start the server (runs on http://localhost:5000/)
   cd ../server
   npm start

   # Start the client (runs on http://localhost:3000/)
   cd ../client
   npm start
   ```
   ```to run all servers at once
   npm run dev
   ```

4. **Configure server settings:**

   - Update `server/server.js` to configure file upload path and other server settings as needed.

5. **Set up environment variables (if applicable):**

   - If your server or client requires environment variables (e.g., API keys, server URLs), create a `.env` file in respective directories (`server/.env`, `client/.env`) and add necessary variables.

6. **Open in browser:**

   - Once both the server and client are running, open your web browser and navigate to `http://localhost:3000/` to use the application.

## Usage

- Choose a file using the file input.
- Click the "Upload" button to start the upload process.
- Monitor the progress bar as the file uploads.
- Once uploaded, the file details (name and image) will be displayed.

## Technologies Used

- **Frontend:**
  - React
  - Axios
  - Bootstrap (for styling)

- **Backend:**
  - Express
  - express-fileupload middleware

## Folder Structure

```
project-root/
├── client/           # Frontend React App
│   ├── public/       # Public assets
│   ├── src/          # React components and App.js
│   └── package.json  # Client dependencies and scripts
│
└── server/           # Backend Express Server
    ├── uploads/      # Uploaded files storage (create if not exists)
    ├── server.js     # Express server configuration
    └── package.json  # Server dependencies and scripts
```

`

