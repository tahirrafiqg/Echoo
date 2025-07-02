# 📍 Field Workforce Management App

A full-featured **MERN + React Native CLI** mobile and web application to manage and track field employees in real-time. This app includes location tracking, live chat, file uploads, job assignment, and an admin dashboard.

---

## 🚀 Tech Stack

| Layer          | Tech                     |
|----------------|--------------------------|
| Mobile         | React Native CLI + TypeScript |
| Web Dashboard  | React + MUI              |
| Backend        | Node.js + Express        |
| Database       | MongoDB + Mongoose       |
| Realtime       | Socket.IO                |
| Maps           | Google Maps SDK (mobile + web) |
| File Storage   | AWS S3                   |
| Auth           | JWT                      |
| Push           | Firebase Cloud Messaging |
| Permissions    | Camera, GPS, Media, Notifications |

---

## 🗺️ Project Phases

### ✅ PHASE 1: Planning & Setup

- Define user roles: Admin, Field Worker
- Set up GitHub repo, folder structure, and `.env` support
- Configure AWS, Firebase, MongoDB Atlas
- Create mobile and backend project scaffolds

---

### ✅ PHASE 2: Backend Setup

**Project Structure**
```
/server
 ┣ /controllers
 ┣ /models
 ┣ /routes
 ┣ /sockets
 ┣ /middleware
 ┣ /utils
 ┣ app.js
 ┗ server.js
```

**Key Features**
- JWT-based Auth (`/auth`)
- Job Assignment APIs (`/jobs`)
- Worker location tracking (`/location`)
- Report upload with image (to S3)
- Realtime chat and location (Socket.IO)
- Firebase push notification handler

---

### ✅ PHASE 3: Mobile App (React Native CLI)

**Screens**
- Login / Register
- Job List
- Job Detail (Map + Info)
- Report Submission (Image + Notes)
- Live Location Tracker
- Realtime Chat

**Key Libraries**
- `@react-navigation/native`
- `react-native-maps`
- `react-native-permissions`
- `react-native-image-picker`
- `socket.io-client`
- `axios`
- `aws-sdk` (or REST upload)

**Permissions**
- Location
- Camera
- Media Library
- Push Notifications

**Realtime Location**
- Background geolocation (e.g., `react-native-background-geolocation`)
- Emit location via socket every few seconds

---

### ✅ PHASE 4: Admin Dashboard (Web)

**Tech:** React + MUI + Socket.IO + Google Maps JS

**Features**
- Login
- Live Worker Map
- Assign Jobs UI
- View Job Reports
- Realtime Admin ↔ Worker Chat

---

### ✅ PHASE 5: Push Notifications (FCM)

- Register device tokens on mobile
- Send push from backend:
  - New Job Assigned
  - Admin Message
  - Job Completed

---

### ✅ PHASE 6: Security & Deployment

- Password hashing with bcrypt
- HTTPS via reverse proxy
- AWS S3: Private bucket + Signed URLs
- MongoDB Atlas for database
- Deploy backend on:
  - Railway / Render / EC2
- App builds via Xcode / Android Studio
- Optional CI/CD with GitHub Actions

---

## 📁 Suggested Mobile Folder Structure

```
/mobile
 ┣ /src
 ┃ ┣ /screens
 ┃ ┣ /components
 ┃ ┣ /api
 ┃ ┣ /sockets
 ┃ ┣ /hooks
 ┃ ┗ /utils
 ┗ App.tsx
```

---

## 🔮 Future Enhancements

- Worker availability status toggle
- Analytics dashboard for admin
- Offline mode + sync queue
- Admin role-based access levels
- Version update notifier for mobile

---

## 🧩 Optional Extras (To be added)

- MongoDB schema definitions
- Socket event flowchart
- Swagger/OpenAPI for REST API
- UI wireframes
- AWS IAM policy for S3 upload

---

## 🧑‍💻 Maintained By

- Built with ❤️ by [Your Name]
- MERN stack + Native mobile enthusiast
