# AI-Powered Resume Builder

A full-stack AI resume builder with a React/Vite front-end and a Node.js/Express back-end. The app helps users create, edit, and review resumes with AI assistance, PDF preview, ATS scoring, and version management.

## Project Structure

- `client/` — React front-end built with Vite
- `server/` — Express back-end with MongoDB, authentication, and AI services

## Features

- Resume editor with sections for experience, education, skills, certifications, and summary
- AI-powered content generation and resume analysis
- PDF resume preview and export support
- Authentication and user session management
- Resume versioning and history

## Requirements

- Node.js 18+ (or compatible)
- npm or yarn
- MongoDB instance
- Environment variables for server configuration and Google AI credentials

## Setup

### 1. Install dependencies

From the project root:

```bash
cd client
npm install

cd ../server
npm install
```

### 2. Configure environment variables

Create a `.env` file in the `server/` folder and add the required variables such as:

```env
PORT=5000
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
GOOGLE_API_KEY=your_google_api_key
GOOGLE_CLIENT_ID=your_google_client_id
GOOGLE_CLIENT_SECRET=your_google_client_secret
```

### 3. Run the app

Start the server:

```bash
cd server
npm run dev
```

Start the client:

```bash
cd client
npm run dev
```

The front-end should be available at the Vite dev server URL, typically `http://localhost:5173`, and the back-end will run on `http://localhost:5000`.

## Scripts

### Client

- `npm run dev` — start Vite development server
- `npm run build` — build production assets
- `npm run preview` — preview production build

### Server

- `npm run start` — run the server
- `npm run dev` — run the server in watch mode

## Notes

- Ensure MongoDB is running and accessible before starting the server.
- The server uses Google AI and auth integrations. Configure credentials based on the environment and project settings.

## License

This repository does not include a license file. Add one if you want to open source this project.
