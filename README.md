# Live Location Tracking Application

A real-time location tracking web application that displays your current location on an interactive map, maintains location history, and provides user authentication.

## Features

- 📱 **Real-time Location Tracking**: Track and display your current location in real-time
- 🗺️ **Interactive Map**: View your location on a map powered by Leaflet/OpenStreetMap
- 🔐 **User Authentication**: Secure login and registration system
- 📜 **Location History**: View your past locations with timestamps
- 🚫 **Offline Support**: Fallback display for when map services are unavailable

## Technology Stack

- **Frontend**: HTML, CSS, JavaScript
- **Backend**: Node.js, Express.js
- **Database**: MongoDB
- **Maps**: Leaflet with OpenStreetMap
- **Authentication**: JWT (JSON Web Tokens)

## Installation

### Prerequisites

- Node.js (v14 or higher)
- MongoDB

### Steps

1. **Clone the repository**

```bash
git clone <repository-url>
cd live-location-tracking
```

2. **Install dependencies**

```bash
pnpm install
```

3. **Set up environment variables**

Create a `.env` file in the root directory with the following variables:

```
PORT=7890
MONGODB_URI=mongodb://localhost:27017/location-tracker
JWT_SECRET=your_jwt_secret_key
```

4. **Start MongoDB**

Make sure MongoDB is running on your system:

```bash
mongod
```

5. **Start the application**

```bash
npm start
```

The application should now be running at http://localhost:7890

## Usage

1. **Register a new account** at http://localhost:7890/register.html
2. **Log in** with your credentials at http://localhost:7890/login.html
3. **Enable location permissions** when prompted by your browser
4. **Track your location** by clicking the "Start Tracking" button
5. **View your location history** at the bottom of the dashboard

## Debugging

If you encounter issues, use the built-in debug tool:

1. Open http://localhost:7890/debug.html
2. Check the server status and API connections
3. Test registration and login functionality
4. View detailed error messages and environment information
