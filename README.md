# Event Management Application

A full-stack event management application built with React (Vite) frontend and Node.js/Express backend. The application allows users to view, create, edit, and delete events.

## Features

- View list of events
- View detailed information for each event
- Create new events
- Edit existing events
- Delete events
- Responsive design
- Optimistic UI updates with React Query
- RESTful API backend with JSON data storage

## Technologies Used

### Frontend
- **React** - JavaScript library for building user interfaces
- **Vite** - Fast build tool and development server
- **React Router** - Declarative routing for React
- **React Query (TanStack Query)** - Data fetching and state management
- **ESLint** - Code linting for quality and consistency

### Backend
- **Node.js** - JavaScript runtime
- **Express.js** - Web framework for building REST APIs
- **body-parser** - Middleware for parsing request bodies

## Project Structure

```
event-management-2/
├── backend/                 # Node.js/Express server
│   ├── app.js               # Express application entry point
│   ├── package.json         # Backend dependencies and scripts
│   └── data/                # JSON data storage
│       ├── events.json      # Events data
│       └── images.json      # Image data
├── public/                  # Static assets
├── src/                     # React source code
│   ├── App.jsx              # Main application component
│   ├── index.css            # Global styles
│   ├── main.jsx             # Entry point
│   ├── assets/              # Images, icons, etc.
│   ├── components/          # Reusable UI components
│   │   ├── Header.jsx       # Application header
│   │   ├── ImagePicker.jsx  # Image upload component
│   │   ├── UI/              # Shared UI elements
│   │   │   ├── ErrorBlock.jsx
│   │   │   ├── LoadingIndicator.jsx
│   │   │   └── Modal.jsx
│   │   └── Events/          # Event-related components
│   │       ├── EditEvent.jsx
│   │       ├── EventDetails.jsx
│   │       ├── EventForm.jsx
│   │       ├── EventItem.jsx
│   │       ├── Events.jsx
│   │       ├── EventsIntroSection.jsx
│   │       ├── FindEventSection.jsx
│   │       ├── NewEvent.jsx
│   │       └── NewEventsSection.jsx
│   └── util/                # Utility functions
│       └── http.js          # HTTP client configuration
├── .gitignore               # Git ignore rules
├── eslint.config.js         # ESLint configuration
├── index.html               # HTML template
├── package.json             # Frontend dependencies and scripts
├── vite.config.js           # Vite configuration
└── README.md                # Project documentation
```

## Setup Instructions

1. **Clone the repository**
   ```bash
   git clone https://github.com/smsatheesh/event-management-2.git
   cd event-management-2
   ```

2. **Install frontend dependencies**
   ```bash
   npm install
   ```

3. **Install backend dependencies**
   ```bash
   cd backend
   npm install
   cd ..
   ```

## Running the Project

### Development Mode

To run both frontend and backend concurrently during development:

1. Start the backend server:
   ```bash
   cd backend
   npm start
   # Server will run on http://localhost:8080
   ```

2. In a new terminal, start the frontend development server:
   ```bash
   npm run dev
   # Frontend will run on http://localhost:5173
   ```

### Production Build

To build the frontend for production:
```bash
npm run build
```

To preview the production build:
```bash
npm run preview
```

## Available Scripts

### Frontend (`package.json`)
- `npm run dev` - Start Vite development server
- `npm run build` - Build for production
- `npm run lint` - Run ESLint
- `npm run preview` - Preview production build

### Backend (`backend/package.json`)
- `npm start` - Start the Express server

## Contributor

- **Satheesh S M** - [https://github.com/smsatheesh](https://github.com/smsatheesh)

## License

This project is open source and available under the MIT License.
