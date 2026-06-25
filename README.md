# The Golden Shutter

A modern full-stack wedding photography booking platform built with the MERN stack, featuring an elegant portfolio gallery, seamless booking experience, secure backend APIs, and cloud-based image management.

## Screenshot

![The Golden Shutter Screenshot](frontend/Screenshots/image.png)

---

## Tech Stack

### Frontend

* React 19
* Vite
* Tailwind CSS
* Axios

### Backend

* Node.js
* Express 5
* MongoDB (Mongoose)
* Cloudinary
* Nodemailer

---

## Necessary NPM Packages

### Frontend

```bash
npm install react react-dom react-router-dom axios
npm install -D vite tailwindcss @tailwindcss/vite eslint
```

### Backend

```bash
npm install express mongoose cors dotenv cloudinary multer multer-storage-cloudinary nodemailer jsonwebtoken bcryptjs cookie-parser express-validator morgan
npm install -D nodemon
```

---

## Quick Start

### Prerequisites

* Node.js v16+
* npm v8+
* MongoDB
* Cloudinary Account

### Installation

```bash
# Clone Repository
git clone <repository-url>

# Navigate to Project
cd THE-GOLDEN-SHUTTER

# Backend
cd backend
npm install

# Frontend
cd ../frontend
npm install
```

### Running

#### Backend

```bash
cd backend
npm start
```

Runs on:

```text
http://localhost:5000
```

#### Frontend

```bash
cd frontend
npm run dev
```

Runs on:

```text
http://localhost:5173
```

### Production Build

```bash
cd frontend
npm run build
```

---

## Color Palette

### Root CSS Variables

| Variable       | Value             | Description     |
| -------------- | ----------------- | --------------- |
| `--bg`         | `#000000`         | Main Background |
| `--text`       | `#FFFFFF`         | Primary Text    |
| `--card`       | `#1F2124`         | Card Background |
| `--border`     | `#69727D`         | Border Color    |
| `--overlay-30` | `rgba(0,0,0,0.3)` | Overlay         |
| `--overlay-10` | `rgba(0,0,0,0.1)` | Overlay         |

### Brand Colors

* `#F5F1E8`
* `#9B7653`
* `#2C2C2C`
* `#6A6A6A`
* `#4A4A4A`

---

## Scripts

| Command         | Description                       |
| --------------- | --------------------------------- |
| `npm start`     | Start Backend Server              |
| `npm run dev`   | Start Frontend Development Server |
| `npm run build` | Build Production Version          |
| `npm run lint`  | Run ESLint                        |

---

## API Endpoints

* `/api/auth`
* `/api/gallery`
* `/api/weddings`
* `/api/bookings`
* `/api/contact`

---

## Environment Setup

Create a `.env` file inside the `backend` folder.

```env
PORT=5000
CLIENT_ORIGIN=http://localhost:5173

MONGO_URI=your_mongodb_connection_string

CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_api_secret

EMAIL_USER=your_email@gmail.com
EMAIL_PASSWORD=your_app_password
```

---

## Features

* Responsive Gallery
* Wedding Booking System
* Contact Form
* Cloudinary Image Management
* Email Notifications
* Authentication System
* REST API
* Modern Responsive UI

---

## Deployment

### Backend (Render)

Configure the following environment variables:

* `PORT`
* `MONGO_URI`
* `CLOUDINARY_CLOUD_NAME`
* `CLOUDINARY_API_KEY`
* `CLOUDINARY_API_SECRET`
* `EMAIL_USER`
* `EMAIL_PASSWORD`

### Frontend (Vercel)

Configure the following environment variable:

```env
VITE_API_URL=your_backend_api_url
```

The frontend communicates with the deployed backend using this API URL.
