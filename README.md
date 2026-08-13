# AI-Powered Interview Preparation Platform

A full-stack web application designed to help job seekers and students prepare for technical and behavioral interviews using Generative AI. The system accepts candidate resumes or skill descriptions alongside target job descriptions to analyze role requirements, compute match alignment scores, and auto-generate tailored interview questions, key concepts to study, and preparation strategies.

---

## 📌 Project Overview

Preparing for specialized technical roles requires understanding specific job requirements and bridging skill gaps effectively. This platform automates interview preparation by evaluating candidate profiles against job descriptions to produce actionable interview prep guides.

### Key Features:
- **Resume & Profile Parsing**: Extracts details from PDF/DOCX resumes or custom self-descriptions.
- **Job Description Analysis**: Parses target job descriptions to identify key technical competencies.
- **Match Score Calculation**: Computes candidate alignment scores (0–100%) against target roles.
- **Tailored Interview Strategy**: Generates role-specific technical questions, behavioral topics, and key areas of improvement.
- **Interactive Prep Dashboard**: Stores previous interview preparation reports for review and tracking.

---

## 🛠️ Tech Stack

### Frontend
- **Framework**: React.js (Vite)
- **Styling**: SCSS / Modern Modular Styling
- **Routing**: React Router v7
- **HTTP Client**: Axios

### Backend
- **Runtime**: Node.js & Express.js
- **Database**: MongoDB (Mongoose ORM)
- **Authentication**: JWT & Cookie-Parser & BcryptJS
- **AI Engine**: Google GenAI SDK (`@google/genai`)
- **Document Parsing**: PDF-Parse & Multer
- **Validation**: Zod Schema Validation

---

## 📁 Repository Structure

```
AI-Powered-Interview-Preparation-Platform/
│
├── Backend/
│   ├── src/
│   │   ├── config/          # Database configuration
│   │   ├── controllers/     # Authentication & Interview controllers
│   │   ├── middlewares/     # JWT authentication & upload middlewares
│   │   ├── models/          # MongoDB schemas (User, Interview, Report)
│   │   ├── routes/          # Express API endpoints
│   │   └── services/        # AI prompt execution & PDF parsing
│   ├── server.js            # Backend entry point
│   └── package.json
│
├── Frontend/
│   ├── src/
│   │   ├── features/        # Auth & Interview pages & components
│   │   ├── style/           # Global SCSS styles
│   │   ├── App.jsx          # Root App component
│   │   └── main.jsx         # React DOM renderer
│   ├── index.html
│   └── package.json
│
└── README.md
```

---

## 💻 Installation & Setup

### Prerequisites
- Node.js (v18 or higher)
- MongoDB instance (local or MongoDB Atlas)

### 1. Clone the Repository
```bash
git clone https://github.com/vivek-singh-18/AI-Powered-Interview-Preparation-Platform.git
cd AI-Powered-Interview-Preparation-Platform
```

### 2. Backend Setup
```bash
cd Backend
npm install
```

Create a `.env` file in the `Backend/` directory:
```env
PORT=5000
MONGO_URI=mongodb://localhost:27017/ai-interview-prep
JWT_SECRET=your_jwt_secret_key
GEMINI_API_KEY=your_google_gemini_api_key
```

Start the backend development server:
```bash
npm run dev
```

### 3. Frontend Setup
```bash
cd ../Frontend
npm install
```

Start the frontend development server:
```bash
npm run dev
```

The application will run on `http://localhost:5173`.

---

## 🧑‍💻 Author

**Vivek**  
*AI-Powered Interview Preparation Platform*  
GitHub: [@vivek-singh-18](https://github.com/vivek-singh-18)
