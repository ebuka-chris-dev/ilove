# ILOVE API

A production-ready backend API for a social and communication platform, built with Node.js and Express.

The platform provides authentication, user management, real-time messaging, social connections, payments, wallets, KYC verification, notifications, moderation, reporting, and other core application services.

### 🌐 Live Project

**Production API:**
https://capatuno.com/

**Interactive API Documentation:**
https://capatuno.com/api-docs/

The API is documented with Swagger/OpenAPI, allowing developers to explore and test available endpoints directly from the browser.

---

## 🚀 Key Features

* 🔐 **Authentication & Authorization**

  * JWT authentication
  * Role-based access control
  * Password hashing
  * Email and phone verification
  * OTP verification

* 👤 **User Management**

  * User registration and profiles
  * User interests
  * Account management
  * User blocking and safety controls

* 💬 **Real-Time Communication**

  * Real-time chat using Socket.IO
  * Private messaging
  * Chat management and moderation
  * Message handling

* 🤝 **Social Features**

  * Friend requests
  * User relationships
  * Interest management
  * User interactions

* 💳 **Payments & Wallets**

  * Wallet management
  * Transaction tracking
  * Payment processing
  * Payment verification
  * Paystack and Flutterwave integrations

* 🪪 **KYC & Verification**

  * KYC verification workflows
  * Verification requests
  * Email verification
  * Phone verification

* 🛡️ **Safety & Moderation**

  * User reporting
  * User blocking
  * Safety bans
  * Chat moderation
  * Administrative moderation tools

* 🔔 **Notifications**

  * Application notification management
  * Email notifications
  * OTP communication

* 🖼️ **Media Management**

  * Image uploads
  * File handling
  * User profile media

---

## 🛠️ Technology Stack

### Backend

* Node.js
* Express.js
* JavaScript
* REST API
* Socket.IO

### Database

* MongoDB
* Mongoose
* PostgreSQL / Sequelize

### Authentication & Security

* JWT
* bcrypt
* CORS
* Environment-based configuration
* Authentication and authorization middleware

### Third-Party Services

* Paystack
* Flutterwave
* Twilio
* Nodemailer

### API Documentation

* Swagger
* OpenAPI

### Deployment

* Docker
* Nginx
* Namecheap VPS
* HTTPS / SSL
* Reverse Proxy

---

## 🏗️ Architecture

The application uses a modular backend structure where major application features are separated into independent domains.

```text
src/
├── config/
├── docs/
├── domains/
│   ├── adminUser/
│   ├── chat/
│   ├── friend_request/
│   ├── interest/
│   ├── kyc_verification/
│   ├── message/
│   ├── notificationLog/
│   ├── paystack/
│   ├── report/
│   ├── safetyBan/
│   ├── transaction/
│   ├── upload_image/
│   ├── user/
│   ├── verificationRequest/
│   ├── wallet/
│   └── wallet_transaction/
├── routes/
├── util/
├── index.js
└── server.js
```

This approach keeps application responsibilities separated and makes the backend easier to maintain and extend.

---

## ☁️ Production Deployment

The API is deployed on a **Namecheap VPS** using Docker and Nginx.

```text
Client
   │
   │ HTTPS
   ▼
Nginx Reverse Proxy
   │
   ▼
Docker Container
   │
   ▼
Node.js / Express API
   │
   ├── MongoDB
   ├── Payment Services
   ├── Email Services
   └── SMS Services
```

The production deployment involved configuring:

* VPS infrastructure
* Docker containerization
* Nginx reverse proxy
* Custom domain
* HTTPS/SSL
* Environment variables
* Production API configuration

---

## 💡 Engineering Highlights

This project demonstrates practical experience with:

* Designing and developing RESTful APIs
* Building authentication and authorization systems
* Working with MongoDB and Mongoose
* Implementing real-time communication with Socket.IO
* Integrating third-party payment services
* Implementing wallet and transaction workflows
* Building verification and KYC processes
* Developing moderation and reporting functionality
* Integrating external email and SMS services
* Documenting APIs with Swagger/OpenAPI
* Containerizing applications with Docker
* Deploying Node.js applications to a VPS
* Configuring Nginx as a reverse proxy
* Securing production services with HTTPS

---

## 💻 Running Locally

### Clone the repository

```bash
git clone https://github.com/ebuka-chris-dev/ilove.git

cd ilove
```

### Install dependencies

```bash
npm install
```

### Configure environment variables

Create a `.env` file and configure the required database, authentication, payment, email, SMS, and application settings.

Example:

```env
PORT=8080
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
```

Additional environment variables may be required depending on the services being used.

### Start the application

```bash
npm start
```

---

## 📚 API Documentation

Explore the complete API through the live Swagger documentation:

**https://capatuno.com/api-docs/**

---

## 👨‍💻 Developer

**Ebuka Christian**

Full-Stack JavaScript Developer specializing in building web applications, REST APIs, real-time systems, database-driven applications, and production deployments.

**GitHub:**
https://github.com/ebuka-chris-dev

---

### 📌 Project

This project represents hands-on experience designing, developing, documenting, and deploying a production backend application using modern JavaScript technologies.
