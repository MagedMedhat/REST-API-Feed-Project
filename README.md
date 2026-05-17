# REST Node.js Project

A full-stack REST API application built with Node.js, Express, MongoDB, and React.

## Project Structure

- `Backend/` - Node.js/Express server with MongoDB integration
- `Frontend/` - React client application
- `package.json` - Root package.json (likely for shared scripts or dependencies)

## Backend Features

- RESTful API endpoints for authentication and feed management
- User authentication with JWT (JSON Web Tokens)
- Image upload functionality using Multer
- Input validation with Express Validator
- MongoDB database integration with Mongoose
- CORS middleware for cross-origin requests
- Error handling middleware

### API Endpoints

#### Authentication
- `POST /auth/login` - User login
- `PUT /auth/signup` - User registration
- `GET /auth/status` - Get user status (protected)
- `PATCH /auth/status` - Update user status (protected)

#### Feed
- `GET /feed/posts` - Get all posts (protected)
- `POST /feed/post` - Create a new post (protected)
- `GET /feed/post/:postId` - Get a specific post (protected)
- `PUT /feed/post/:postId` - Update a post (protected)
- `DELETE /feed/post/:postId` - Delete a post (protected)

## Frontend Features

- React-based user interface
- Authentication flow (login/register)
- Feed display and post management
- Image upload capability
- Responsive design

## Setup Instructions

### Prerequisites
- Node.js (v14+ recommended)
- MongoDB instance (local or cloud)
- npm or yarn package manager

### Backend Setup
1. Navigate to the Backend directory:
   ```bash
   cd Backend
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the server:
   ```bash
   npm start
   ```
   or for development with nodemon:
   ```bash
   npm run dev
   ```

### Frontend Setup
1. Navigate to the Frontend directory:
   ```bash
   cd Frontend
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the development server:
   ```bash
   npm start
   ```
NOTE: This Frontend is OUTDATED. DON'T USE IT

## Environment Variables

The backend requires the following environment variables in a `.env` file:
- `PORT` - Server port (default: 8080)
- `MONGODB_URI` - MongoDB connection string

## Technologies Used

### Backend
- Node.js
- Express.js
- MongoDB with Mongoose
- JWT for authentication
- Multer for file uploads
- Express Validator for input validation
- dotenv for environment variable management

### Frontend
- React
- (Additional frontend technologies would be listed based on package.json)

## API Response Format

All API responses follow a consistent format:
```json
{
  "message": "Success or error message",
  "data": {...} // Optional data payload
}
```

Error responses include appropriate HTTP status codes.

## Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Open a pull request

## License

This repository is open-source and available under the MIT License.