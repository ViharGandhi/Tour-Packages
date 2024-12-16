# Tour Package Booking Application

## Project Description

A full-stack web application for booking tour packages, allowing users to browse available tours, make bookings, and enabling administrators to manage packages and view booking requests.

## Live Demo

🌐 **Website**: [https://tour-package-frontend.onrender.com/](https://tour-package-frontend.onrender.com/)

## Technologies Used

- **Frontend**: React.js (Vite)
- **Styling**: TailwindCSS
- **Backend**: Node.js + Express.js
- **Database**: MongoDB
- **Image Storage**: Appwrite

## Features

### User-Facing Features
- Browse available tour packages
- View detailed package information
- Book tour packages
- Submit booking requests with validation
- Generate booking invoices

### Admin Features
- Add new tour packages
- Update existing packages
- Delete packages
- View all booking requests

## Prerequisites

Before you begin, ensure you have the following installed:
- Node.js (v16 or later)
- npm or yarn
- MongoDB
- Appwrite account

## Setup Instructions

### 1. Clone the Repository

```bash
git clone 
cd 
```

### 2. Frontend Setup (client/travel-app)

```bash
# Navigate to frontend directory
cd client/travel-app

# Install dependencies
npm install

# Create .env file with necessary environment variables
# Example .env contents:
# VITE_BACKEND_URL=http://localhost:5000
# VITE_PROJECT_ID=your_appwrite_project_id
# VITE_BUCKETT_ID=your_appwrite_bucket_id

# Start development server
npm run dev
```

### 3. Backend Setup (server)

```bash
# Navigate to backend directory
cd server

# Install dependencies
npm install

# Create .env file with necessary environment variables
# Example .env contents:
# PORT=5000
# URI=your_mongodb_connection_string

# Start backend server
npm start
```

## Environment Variables

### Frontend (client/travel-app/.env)
- `VITE_BACKEND_URL`: Backend API base URL
- `VITE_PROJECT_ID`: Appwrite Project ID
- `VITE_BUCKETT_ID`: Appwrite Bucket ID

### Backend (server/.env)
- `PORT`: Port number for the backend server
- `URI`: MongoDB connection string

## API Endpoints

### Package Endpoints
- `GET /packages`: Retrieve all tour packages
- `GET /packages/:id`: Retrieve specific package details

### Booking Endpoints
- `POST /bookings`: Submit a package booking

### Admin Endpoints
- `POST /admin/packages`: Add a new package
- `PUT /admin/packages/:id`: Update an existing package
- `DELETE /admin/packages/:id`: Delete a package

## Deployment

### Frontend
- Deployed on Render
- URL: [https://tour-package-frontend.onrender.com/](https://tour-package-frontend.onrender.com/)

### Backend
- Deployed on Render
- URL : [https://tour-package-backend.onrender.com/]

## Additional Notes
- Basic admin authentication is implemented
- Invoices are generated upon successful booking
- Image storage is managed via Appwrite




```
