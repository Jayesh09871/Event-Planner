# Event Planner MERN Stack Project

## Description
Event Planner is a full-stack web application built using the MERN (MongoDB, Express.js, React.js, Node.js) stack. It allows users to create, manage, and participate in events. The application provides user authentication, event scheduling, real-time notifications, and an intuitive user interface.

---

## Features

### 1. User Authentication
- **Sign up** and **Login** functionality.
- Secure password storage using bcrypt.
- Authentication managed using JSON Web Tokens (JWT).

### 2. Event Management
- Create, update, and delete events.
- List and filter events by category, date, or location.
- View event details.

### 3. User Participation
- RSVP to events.
- Track your participation in an event dashboard.

### 4. Real-Time Notifications
- Receive notifications for upcoming events or updates via Socket.io.

### 5. Admin Panel
- Manage all users and events.
- Approve or reject event submissions.

### 6. Responsive Design
- Fully responsive interface for both desktop and mobile users.

---

## Tech Stack

### Frontend
- **React.js** with Hooks and Context API for state management.
- **CSS Modules** for component-based styling.
- **React Router** for navigation.

### Backend
- **Node.js** with **Express.js** framework for building the RESTful API.
- **Socket.io** for real-time notifications.

### Database
- **MongoDB** for storing user and event data.
- **Mongoose** for object modeling.

---

## Installation

### Prerequisites
- Node.js and npm installed.
- MongoDB installed and running locally or via cloud (MongoDB Atlas).

### Steps

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/event-planner.git
   cd event-planner
   ```

2. **Install dependencies:**
   ```bash
   # Install server dependencies
   cd server
   npm install

   # Install client dependencies
   cd ../client
   npm install
   ```

3. **Set up environment variables:**
   Create a `.env` file in the `server` directory and add the following:
   ```env
   MONGO_URI=your-mongodb-connection-string
   JWT_SECRET=your-jwt-secret
   PORT=5000
   ```

4. **Start the application:**
   ```bash
   # Start the backend server
   cd server
   npm run dev

   # Start the frontend
   cd ../client
   npm start
   ```

5. Open the application in your browser at `http://localhost:3000`.

---

## Folder Structure

```
Event-Planner/
├── client/             # Frontend code
│   ├── public/         # Static files
│   └── src/            # React components and pages
├── server/             # Backend code
│   ├── config/         # Database and server configurations
│   ├── models/         # Mongoose models
│   ├── routes/         # API routes
│   └── utils/          # Utility functions
└── README.md           # Project documentation
```

---

## API Endpoints

### Authentication
- `POST /api/auth/register` - Register a new user.
- `POST /api/auth/login` - Log in a user.

### Events
- `GET /api/events` - Fetch all events.
- `POST /api/events` - Create a new event.
- `PUT /api/events/:id` - Update an event.
- `DELETE /api/events/:id` - Delete an event.

### Users
- `GET /api/users` - Fetch all users (admin only).

---

## Future Enhancements
- Add a chat feature for event participants.
- Implement payment integration for paid events.
- Support for event reminders via email or SMS.

---

## License
This project is licensed under the MIT License. See the `LICENSE` file for details.

---

## Author
Developed by [Your Name](https://github.com/your-username).