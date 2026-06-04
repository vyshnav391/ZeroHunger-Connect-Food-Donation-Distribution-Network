# ZeroHunger-Connect-Food-Donation-Distribution-Network
## Overview

HopeBridge is a full-stack web application developed to reduce food wastage and improve food accessibility by connecting food donors with NGOs through a centralized platform.

The system enables donors to register food donations, NGOs to manage and accept available donations, and administrators to monitor the entire redistribution process. The platform focuses on improving coordination, transparency, and efficiency in food distribution.

---

## Problem Statement

Food wastage remains a major challenge despite the increasing demand for food assistance in many communities.

Common issues include:

- Lack of a centralized donation management system
- Manual communication between donors and NGOs
- Delayed food collection and distribution
- Absence of donation tracking mechanisms
- Limited visibility into food redistribution activities

As a result, a significant amount of edible food is discarded before it can reach those in need.

---

## Proposed Solution

HopeBridge provides a centralized digital platform that streamlines food donation and redistribution activities.

The platform allows:

- Donors to register surplus food donations
- NGOs to view and manage available donations
- Administrators to oversee platform operations
- Real-time tracking of donation activities
- Secure and role-based user access

This approach improves efficiency and minimizes food wastage through a structured and transparent workflow.

---

## Features

### User Authentication

- User Registration
- Secure Login
- JWT Authentication
- Role-Based Authorization

### Donor Module

- Create Food Donations
- View Donation History
- Update Donation Information
- Track Donation Status

### NGO Module

- View Available Donations
- Accept Donation Requests
- Manage Distribution Activities
- Monitor Active Donations

### Admin Module

- Manage Users
- Monitor Donations
- View Platform Statistics
- Generate Reports

### Tracking System

- Donation Status Monitoring
- Distribution Tracking
- Historical Records Management

### Security

- Password Encryption using bcrypt
- JWT-Based Authentication
- Protected API Routes

---

## Technology Stack

### Frontend

- React.js
- Vite
- Tailwind CSS

### Backend

- Node.js
- Express.js

### Database

- MongoDB

### Authentication

- JWT (JSON Web Token)
- bcrypt

---

## System Workflow

```text
Donor
   │
   ▼
Create Donation
   │
   ▼
Database Storage
   │
   ▼
NGO Views Donation
   │
   ▼
NGO Accepts Request
   │
   ▼
Food Collection
   │
   ▼
Food Distribution
```

---

## System Architecture

```text
+--------------------+
|       Donor        |
+--------------------+
          |
          v
+--------------------+
|   React Frontend   |
+--------------------+
          |
          v
+--------------------+
| Express REST APIs  |
+--------------------+
          |
          v
+--------------------+
|     MongoDB        |
+--------------------+
          |
          v
+--------------------+
|  NGO / Admin Panel |
+--------------------+
```

---

## Project Structure

```text
HopeBridge/
│
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── hooks/
│   │   ├── services/
│   │   └── assets/
│   │
│   └── package.json
│
├── backend/
│   ├── controllers/
│   ├── routes/
│   ├── models/
│   ├── middleware/
│   ├── config/
│   └── server.js
│
├── screenshots/
│
├── README.md
├── package.json
└── .gitignore
```

---

## Installation

### Clone Repository

```bash
git clone <repository-url>
```

### Navigate to Project Directory

```bash
cd HopeBridge
```

### Install Dependencies

```bash
npm install
```

### Configure Environment Variables

Create a `.env` file inside the backend directory.

```env
MONGODB_URI=your_connection_string
JWT_SECRET=your_secret_key
PORT=5000
```

### Run Backend

```bash
npm start
```

### Run Frontend

```bash
npm run dev
```

---

## Screenshots

Add screenshots inside the `screenshots` directory.

```text
screenshots/
├── login-page.png
├── donor-dashboard.png
├── ngo-dashboard.png
├── admin-dashboard.png
└── donation-history.png
```

---

## Future Enhancements

- Mobile Application Support
- Location-Based Donation Matching
- Route Optimization
- Real-Time Notifications
- Analytics Dashboard
- AI-Based Demand Forecasting

---

## Conclusion

HopeBridge provides a structured and scalable solution for food redistribution by connecting donors, NGOs, and administrators through a unified platform. The system improves transparency, reduces food wastage, and enables efficient coordination throughout the donation lifecycle.
