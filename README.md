# 🐵 Auditing Monkey

An AI-powered Website QA Testing & Exploration Platform that automatically audits websites by crawling pages, clicking buttons, exploring links, capturing screenshots, and generating reports.

---

## 🚀 Overview

Auditing Monkey helps developers, QA engineers, and product teams automate website testing.

Instead of manually navigating through a website, Auditing Monkey uses browser automation to:

- Explore web pages
- Discover links
- Click buttons
- Capture screenshots
- Detect broken links
- Generate audit reports
- Provide real-time scan updates

---

## ✨ Features

### 🔍 Automated Website Crawling
- Opens the target website
- Discovers internal and external links
- Tracks visited pages

### 🖱️ Intelligent Button Exploration
- Finds buttons automatically
- Simulates user interactions
- Records exploration results

### 📸 Screenshot Capture
- Captures screenshots during audits
- Stores visual evidence of scans

### 📊 Real-Time Monitoring
- Live scan updates using Socket.IO
- Displays crawling progress instantly

### ⚠️ Broken Link Detection
- Identifies inaccessible pages
- Generates error reports

### 📄 Report Generation
- Produces structured audit reports
- Summarizes findings and issues

---

## 🏗️ System Architecture

```text
User
 │
 ▼
React Frontend (Vercel)
 │
 ▼
Express API (Node.js)
 │
 ▼
Playwright Automation Engine
 │
 ├── Website Crawling
 ├── Link Exploration
 ├── Button Testing
 ├── Screenshot Capture
 └── Report Generation
```

---

## 🛠️ Tech Stack

### Frontend
- React.js
- Vite
- Axios
- Socket.IO Client

### Backend
- Node.js
- Express.js
- Socket.IO

### Automation
- Playwright

### Deployment
- Vercel
- Railway

---

## 📂 Project Structure

```text
Auditing-Monkey
│
├── backend
│   ├── controllers
│   ├── routes
│   ├── services
│   ├── screenshots
│   ├── reports
│   ├── server.js
│   └── package.json
│
├── frontend
│   ├── src
│   │   ├── components
│   │   ├── pages
│   │   ├── services
│   │   └── App.jsx
│   └── package.json
│
├── electron
│   └── main.js
│
└── README.md
```

---

## ⚙️ Installation

### Clone Repository

```bash
git clone https://github.com/your-username/Auditing-Monkey.git
cd Auditing-Monkey
```

---

### Backend Setup

```bash
cd backend

npm install

npx playwright install chromium

npm start
```

Backend runs on:

```text
http://localhost:5000
```

---

### Frontend Setup

```bash
cd frontend

npm install

npm run dev
```

Frontend runs on:

```text
http://localhost:5173
```

---

## 🚀 Usage

1. Open the application
2. Enter a website URL
3. Click **Start Scan**
4. Monitor real-time exploration
5. Review generated reports and screenshots

---

## 📡 API Endpoint

### Start Website Scan

```http
POST /api/scan
```

Request Body:

```json
{
  "url": "https://example.com"
}
```

Response:

```json
{
  "success": true,
  "message": "Scan started"
}
```

---

## 📈 Future Enhancements

- AI-powered bug detection
- Accessibility auditing
- Form validation testing
- Performance testing
- PDF report export
- Team collaboration dashboard
- SaaS multi-tenant architecture

Auditing Monkey demonstrates:

- Browser automation
- Real-time monitoring
- Website auditing

## 👨‍💻 Authors

### Manoj Aravind S, Bharathi Mohan S, Ajeaay Vishwha V S

Project developed as an automated QA and website auditing platform using Playwright, React, Node.js, and Socket.IO.

