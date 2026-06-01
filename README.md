# EventSeat

EventSeat is a full-stack MERN application built for seamless event discovery and ticket booking. It features user authentication, a smart booking queue, automated email notifications, and an administrative dashboard for event organizers to manage free and paid events.

## Tech Stack
- **Frontend**: React.js, Tailwind CSS, Vite
- **Backend**: Node.js, Express.js
- **Database**: MongoDB (Mongoose ODM)
- **Security**: JWT, Bcrypt, and 2FA OTP Email Verification

## Features
- **User Authentication**: Secure registration and login featuring JWT-based session management.
- **Smart Booking System**: Real-time seat availability updates and double-booking protection.
- **Admin Control Panel**: Interface for event creation, booking approvals/cancellations, and analytics.
- **Email Notifications**: Automatic ticket receipt and registration alerts powered by Nodemailer.
- **Responsive Interface**: Polished UI built with React and Tailwind CSS.

## Installation & Setup

1. **Clone the repository**:
   ```bash
   git clone https://github.com/souvik-bt/event-seat.git
   cd event-seat
   ```

2. **Configure Environment Variables**:
   Create a `.env` file in the `server` directory and configure the following keys:
   ```env
   MONGO_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret
   EMAIL_USER=your_email@gmail.com
   EMAIL_PASS=your_gmail_app_password
   PORT=5000
   ```

3. **Install Dependencies**:
   Navigate to the root directory and install dependencies for both the backend and client:
   ```bash
   npm run install:all
   ```

4. **Seed Database (Optional)**:
   You can populate the database with dummy events and users using the seed script:
   ```bash
   npm run seed --prefix server
   ```

5. **Start Dev Servers**:
   Run both client and server development environments with a single command:
   ```bash
   npm run dev
   ```
