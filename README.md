# React Quiz Application

A modern, interactive quiz application built with React. This application allows users to take quizzes, view their scores, and track their progress.

## Features

- Interactive quiz interface
- Real-time score tracking
- Multiple choice questions
- Progress tracking
- Responsive design

## Technologies Used

- React 19
- JSON Server for data management
- React Testing Library for testing
- Web Vitals for performance monitoring

## Getting Started

### Prerequisites

- Node.js (v14 or higher)
- npm (v6 or higher)

### Installation

1. Clone the repository:

```bash
git clone [your-repository-url]
cd react-quiz
```

2. Install dependencies:

```bash
npm install
```

3. Start the development servers:

```bash
# Start the JSON Server (in one terminal)
npm run server

# Start the React development server (in another terminal)
npm start
```

**Important Note:** You must run both servers simultaneously. The JSON Server (`npm run server`) is essential as it provides the quiz data to the application. Without running the JSON Server, the application will not be able to fetch or display any quiz questions.

The application will be available at [http://localhost:3000](http://localhost:3000)

## Available Scripts

- `npm start` - Runs the app in development mode
- `npm test` - Launches the test runner
- `npm run build` - Builds the app for production
- `npm run server` - Starts the JSON Server for quiz data (Required for data access)
- `npm run eject` - Ejects from Create React App (one-way operation)

## Project Structure

```
react-quiz/
├── src/
│   ├── components/     # React components
│   ├── index.js       # Application entry point
│   └── index.css      # Global styles
├── data/
│   └── questions.json # Quiz questions data
├── public/            # Static assets
└── package.json       # Project dependencies and scripts
```

## Development

The application uses JSON Server to serve quiz data. The server runs on port 8000 and serves the questions from `data/questions.json`. This is a crucial part of the application setup as it:

- Provides a RESTful API for the quiz questions
- Enables data persistence during development
- Allows the React application to fetch and display quiz content
- Must be running alongside the React development server

Without the JSON Server running, the application will not be able to access any quiz data and will fail to function properly.

## Testing

Run the test suite with:

```bash
npm test
```

## Building for Production

To create a production build:

```bash
npm run build
```

This will create an optimized production build in the `build` folder.
