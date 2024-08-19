# 🎥 Movie Ticket Booking Web Application

This repository contains a web application for booking movie tickets online. The project is built using **HTML**, **CSS**, **JavaScript**, and **Node.js**. The application follows a modular architecture with separate **client** and **server** folders to manage frontend and backend code.

## 📂 Project Structure

```bash
movie-ticket-booking/
├── client/
│   ├── public/               # Static assets like images, CSS files, etc.
│   ├── src/
│   │   ├── index.html        # Main HTML file
│   │   ├── style.css         # Styling for the application
│   │   ├── app.js            # Client-side JavaScript logic
├── server/
│   ├── src/
│   │   ├── app.js            # Main server-side code (Node.js + Express)
│   │   ├── routes.js         # API routes for handling movie and booking requests
│   │   ├── database.js       # Database connection and models
│   ├── package.json          # Node.js dependencies for the server
├── .gitignore
├── README.md
├── package.json              # Node.js dependencies for the whole project
```

## 🌟 Features

- **Movie Listing**: Browse available movies, view movie details such as timings, seats, etc.
- **Ticket Booking**: Select movie, time, and seat and proceed to book tickets.
- **User Authentication**: Login and sign-up functionality for users.
- **Responsive Design**: Works seamlessly across various screen sizes.
- **REST API**: Backend built using Node.js and Express, with RESTful routes for handling movie and booking data.

## 🚀 Getting Started

### Prerequisites

Make sure you have the following installed on your local machine:
- **Node.js** (v14 or higher)
- **npm** or **yarn** for dependency management

### Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/movie-ticket-booking.git
   cd movie-ticket-booking
   ```

2. **Install dependencies for both client and server**:

   For the **client**:
   ```bash
   cd client
   npm install
   ```

   For the **server**:
   ```bash
   cd ../server
   npm install
   ```

### Running the Application

1. **Start the server**:
   The server-side code (Node.js) is located in the `server/` folder and handles API requests and the database.

   To run the server:
   ```bash
   cd server
   npm run dev
   ```

   This will start the Node.js server, typically on port `3000`.

2. **Run the client**:
   The client-side code (HTML, CSS, JS) is located in the `client/` folder. You can serve the client using a simple HTTP server like `live-server` or any other tool of your choice.

   Example using **live-server**:
   ```bash
   cd client
   live-server
   ```

   Or, use an `npm` script defined in `client/package.json` to serve the static files:
   ```bash
   npm start
   ```

3. **Open the application**:
   Open a browser and navigate to `http://localhost:8080` (or the port used by your client).

## 🛠️ Technologies Used

- **Frontend (Client)**:
  - **HTML5**: Structure of the web pages.
  - **CSS3**: Styling and layout of the web pages.
  - **JavaScript**: Client-side interactivity and logic.

- **Backend (Server)**:
  - **Node.js**: JavaScript runtime for building the server.
  - **Express**: Web framework for creating RESTful APIs.
  - **MongoDB / MySQL**: Database to store movie and booking information (depending on your choice).

## 🔌 API Endpoints

Here are some of the key API routes exposed by the server (Express):

- `GET /movies`: Fetch a list of available movies.
- `GET /movies/:id`: Fetch details of a single movie.
- `POST /bookings`: Create a new ticket booking.
- `GET /bookings`: Get all bookings for the logged-in user.
- `POST /auth/login`: User login.
- `POST /auth/signup`: User registration.

## 🛡️ Security and Authentication

This app includes user authentication for booking tickets:
- **JWT (JSON Web Token)**: Used for managing user sessions and securing API routes.
- **Password Hashing**: Passwords are hashed before being stored in the database to ensure security.

## 💡 Future Enhancements

- **Payment Integration**: Add functionality for online payment for booked tickets.
- **Movie Reviews**: Users can leave reviews for movies.
- **Seat Availability**: Show real-time seat availability using WebSockets.
- **Push Notifications**: Alert users for upcoming shows they have booked.

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🤝 Contributions

Contributions are welcome! If you'd like to contribute, please fork the repository, create a new branch, and submit a pull request.
