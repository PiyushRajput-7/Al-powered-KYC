# Al-powered-kyc 
Infosys_AI_KYC_Compliance
Repository navigation
Code
Issues
Pull requests
1
 (1)
AI Powered KYC compliance for document verification

License
 MIT license
Code of conduct
 Code of conduct
 3 stars
 2 forks
 0 watching
 3 Branches
 0 Tags
 Activity
Public repository
SannidhiSriram-06/Infosys_AI_KYC_Compliance
Name	
ankushsans
ankushsans
5 days ago
backend
2 weeks ago
frontend
2 weeks ago
notebooks
last week
trained models
5 days ago
CODE_OF_CONDUCT.md
last month
Dataset Information
last month
LICENSE
last month
README.md
2 weeks ago
Repository files navigation
README
AI-Powered KYC & AML Compliance System
An end-to-end AI system for identity document verification, address validation, and fraud detection for BFSI (Banking, Financial Services, and Insurance) workflows. This project leverages Computer Vision, NLP, and a robust MERN stack backend to automate KYC compliance.

Features
User Authentication: Secure registration and login using JWT and Bcrypt.
AI Document Classification: Automatically detects and classifies Aadhaar, PAN, and Passports.
Document Verification: Upload and process identity documents with real-time feedback.
KYC History: Track all past verification attempts with detailed status and results.
OCR Integration: (In Progress) Text extraction for automated data entry.
Modern Dashboard: Responsive UI with glassmorphism and real-time analysis insights.
Project Structure
frontend/: React + Vite application (User Interface).
backend/: Node.js + Express + MongoDB (API Service).
notebooks/: AI/ML research and model training (TensorFlow/Keras).
Tech Stack
Frontend: React.js, React Router, Vanilla CSS, Vite.
Backend: Node.js, Express.js, MongoDB (Mongoose), JWT, Multer.
ML/AI: TensorFlow, Keras, OpenCV, Gradio, OpenBharatOCR.
Getting Started
1. Prerequisites
Node.js (v18+)
MongoDB (Running locally or Atlas cloud instance)
Python 3.9+ (For ML notebooks)
2. Backend Setup
cd backend
npm install
Create a .env file in the backend/ directory:

PORT=5000
MONGODB_URI=mongodb://localhost:27017/kyc_db
JWT_SECRET=your_super_secret_key
NODE_ENV=development
Start the backend server:

npm run dev
3. Frontend Setup
cd frontend
npm install
npm run dev
Open http://localhost:5173 in your browser.

🛰️ API Endpoints
Authentication
POST /api/auth/register - Create a new account.
POST /api/auth/login - Authenticate user and get token.
KYC Operations (Requires Auth)
POST /api/kyc/verify - Upload identity and supporting documents.
GET /api/kyc/history - Retrieve a user's verification history.
ML Integration
The classification models are located in notebooks/. To run the ML service interface:

Navigate to notebooks/.
Open KYC Identification for Aadhar, Pan and Passport.ipynb.
Run the Gradio interface cells to start the prediction API.
