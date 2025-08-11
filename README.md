# Mini Context API Demo

A simple React application demonstrating the Context API pattern for state management. This project showcases how to share user authentication state across components without prop drilling.

## What This Project Does

This mini Context API demo implements a basic login system that demonstrates:

- **Context Creation**: Creating a UserContext to hold user authentication state
- **Context Provider**: Wrapping the application with UserContextProvider to provide user state
- **State Management**: Managing user login state (username and password) across components
- **Context Consumption**: Using useContext hook to access user data in different components

## Features

- Login form with username and password fields
- Profile component that displays welcome message when logged in
- Conditional rendering based on authentication state
- Clean separation of concerns using Context API pattern

## Project Structure

```
src/
├── components/
│   ├── Login.jsx          # Login form component
│   └── Profile.jsx        # Profile display component
├── context/
│   ├── UserContext.js     # Context definition
│   └── UserContextProvider.jsx  # Context provider component
├── App.jsx               # Main application component
└── main.jsx             # Application entry point
```

## How It Works

1. **UserContext**: Creates a React context for sharing user state
2. **UserContextProvider**: Manages user state and provides it to child components
3. **Login Component**: Captures user credentials and updates the context state
4. **Profile Component**: Displays user information if logged in, otherwise shows login prompt

## Getting Started

1. Clone the repository
2. Install dependencies: `npm install`
3. Start the development server: `npm run dev`
4. Open your browser and navigate to `http://localhost:5173`

## Built With

- React 18
- Vite
- Context API for state management
