# mern-screen---recorder
🎥 Screen Recorder App (MERN) — A full-stack web app to record browser tab + microphone audio, preview, download, and upload recordings to a Node.js + SQL backend. Includes recordings list with playback support. Built as part of a take-home MERN assignment.

<img width="1914" height="1016" alt="image" src="https://github.com/user-attachments/assets/41e40f50-64ca-4113-b837-0cb707ba7895" />
# 🎥 Screen Recorder App (MERN)

## 📌 Overview
This is a full-stack **MERN Take-Home Assignment** project where users can:
- Record the **current browser tab** with microphone audio.
- Preview and download the recording (max duration: 3 minutes).
- Upload the recording to a **Node.js + Express + SQL backend**.
- View a list of uploaded recordings with inline playback, file size, and created date.

The project demonstrates integration of **modern frontend APIs** (`navigator.mediaDevices`, `MediaRecorder`) with a simple **backend for file storage & metadata**.

---

## ✨ Features
- 🎥 **Screen + Audio Recording** (browser tab + microphone)
- ⏱️ **Live Timer** during recording (auto-stop at 3 minutes)
- ▶️ **Preview & Playback** after stopping
- 💾 **Download Option** for recordings
- ☁️ **Upload to Backend** (Express API + SQL DB)
- 📂 **Recordings List Page** with:
  - Title
  - Size
  - Created Date
  - Inline Play Support

---

## 🛠️ Tech Stack
### Frontend
- **React / Vanilla JS**
- Media APIs: `navigator.mediaDevices.getDisplayMedia`, `MediaRecorder`

### Backend
- **Node.js + Express**
- **SQLite / SQL database** for metadata storage
- Multer for file uploads

### Deployment
- **Frontend**: Vercel / Netlify
- **Backend**: Render
- **Database**: SQL (SQLite for local, PostgreSQL/MySQL for cloud)

---

## 🚀 Getting Started

### 1️⃣ Clone the repo
```bash
git clone https://github.com/<your-username>/screen-recorder-app.git
cd screen-recorder-app
3️⃣ Frontend Setup

Simple HTML frontend — run with:

cd frontend
serve .


Frontend runs on http://localhost:3000

4️⃣ Usage

Click Start Recording

Allow permissions → record screen + mic

Click Stop Recording

Preview, Download, or Upload to backend

Check Recordings List page

📂 API Endpoints

POST /api/recordings → Upload new recording

GET /api/recordings → Fetch list of recordings

GET /api/recordings/:id → Fetch a specific recording

🔮 Future Enhancements

🌐 Upload recordings to Cloud Storage (AWS S3 / Cloudinary)

🛡️ User Authentication for secure uploads

📱 Mobile responsive UI

📊 Recording analytics (duration, usage stats)

⚠️ Known Limitations

Works best on Google Chrome (due to getDisplayMedia support).

Local storage is SQLite; for production, use Postgres/MySQL.

No user login/authentication (public upload).

👨‍💻 Author

Developed by Yeddula Ganesh Maruthi ✨
Part of MERN Take-Home Assignment.
