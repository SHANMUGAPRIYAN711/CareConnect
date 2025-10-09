project:
  name: CareConnect
  tagline: "Centralized Hospital Management and Appointment System"
    CareConnect is a full-stack web-based hospital management system designed to streamline
    the process of online appointment booking, doctor-patient interaction, and administrative
    hospital operations. It provides three key user roles — Admin, Doctor, and Patient — with
    secure authentication, efficient scheduling, and AI-assisted features like voice-based
    appointment booking.

repository:
  url: "https://github.com/SHANMUGAPRIYAN711/CareConnect"
  structure:
    - admin/: "Admin dashboard and configuration module"
    - backend/: "Server-side logic, APIs, and database integration"
    - frontend/: "User interface (React or web components)"
    - vercel.json: "Deployment configuration for hosting"
    - README.yaml: "Documentation file"

roles:
  admin:
    - Secure login and access control
    - CRUD operations for doctor profiles
    - Manage all appointments and reports
    - Monitor hospital activities via dashboard
  doctor:
    - Secure login and dashboard
    - View scheduled appointments
    - Manage personal profile and availability
    - Track earnings and performance
  patient:
    - Registration and authentication
    - Search and filter doctors by specialization
    - Book appointments within a 7-day window
    - Voice-based appointment booking via AI
    - View appointment history

tech_stack:
  frontend:
    - React.js
    - HTML, CSS, JavaScript
  backend:
    - Node.js
    - Express.js
  database:
    - MongoDB (Mongoose)
  authentication:
    - JWT (JSON Web Token)
    - bcrypt (for password hashing)
  payment_gateways:
    - Stripe
    - Razorpay
  deployment:
    - Vercel / Render / MongoDB Atlas
  version_control:
    - Git and GitHub

backend_dependencies:
  - bcrypt: "Password hashing"
  - cloudinary: "Image storage"
  - cors: "Cross-origin requests"
  - dotenv: "Environment variable management"
  - express: "Web framework for Node.js"
  - jsonwebtoken: "Authentication using JWT"
  - mongoose: "ODM for MongoDB"
  - multer: "File uploads"
  - nodemon: "Development auto-restart"
  - razorpay: "Payment integration"
  - stripe: "Payment integration"
  - validator: "Data validation"

installation:
  prerequisites:
    - Node.js (v16 or above)
    - npm or yarn
    - MongoDB (local or Atlas)
  steps:
    - Step 1: Clone the repository
      command: "git clone https://github.com/SHANMUGAPRIYAN711/CareConnect.git"
    - Step 2: Install backend dependencies
      path: "cd backend"
      command: "npm install"
    - Step 3: Create an .env file with the following variables
      env_variables:
        - PORT=5000
        - DB_URI=your_mongodb_connection_string
        - JWT_SECRET=your_jwt_secret
        - STRIPE_KEY=your_stripe_secret
        - RAZORPAY_KEY_ID=your_razorpay_key
        - RAZORPAY_KEY_SECRET=your_razorpay_secret
    - Step 4: Run the backend server
      command: "npm run server"
    - Step 5: Setup frontend
      path: "../frontend"
      command: "npm install && npm start"

usage_flow:
  patient:
    - Register or login
    - Browse doctors by specialization
    - Choose available date and time within 7 days
    - Confirm booking (voice-enabled option available)
    - View appointment confirmation
  doctor:
    - Login to personal dashboard
    - View upcoming appointments
    - Manage schedules and patient data
    - Track earnings
  admin:
    - Login to admin dashboard
    - Manage doctors and patient appointments
    - Generate performance and booking reports

environment_variables:
  backend:
    - PORT: "Backend server port"
    - DB_URI: "MongoDB connection string"
    - JWT_SECRET: "JWT signing key"
    - STRIPE_KEY: "Stripe secret key"
    - RAZORPAY_KEY_ID: "Razorpay API key"
    - RAZORPAY_KEY_SECRET: "Razorpay API secret"
    - EMAIL_USER: "SMTP email ID (optional)"
    - EMAIL_PASS: "SMTP password (optional)"
  frontend:
    - REACT_APP_API_URL: "Backend API base URL"

features_summary:
  - Role-based authentication and authorization
  - Secure password encryption
  - Voice AI booking for accessibility
  - Appointment filtering and scheduling
  - Doctor specialization search
  - Real-time database interaction
  - Integrated payment gateways
  - Scalable modular architecture

future_enhancements:
  - Real-time notifications using Socket.IO
  - Email/SMS reminders for appointments
  - Electronic Health Record (EHR) integration
  - Role expansion: Nurse & Lab modules
  - Analytics dashboard for admins
  - AI-powered doctor recommendations
  - Dark/light mode support in UI

credits:
  author: "Shanmugapriyan"
  github: "https://github.com/SHANMUGAPRIYAN711"
  collaborators: []
  license: "MIT License"
  acknowledgements:
    - Node.js and Express.js
    - MongoDB Atlas
    - Razorpay and Stripe APIs
    - React.js community

insight:
  summary: >
    CareConnect bridges the gap between patients and healthcare providers through an intuitive,
    cloud-based web solution. It enhances user accessibility, automates appointment management,
    and offers a scalable architecture that can be adapted for hospitals, clinics, and
    telemedicine systems.
  objective: >
    To centralize hospital operations and deliver a modern healthcare experience through
    AI-driven and cloud-integrated solutions.
  vision: >
    A connected healthcare ecosystem where patients, doctors, and administrators collaborate
    seamlessly for better outcomes.
