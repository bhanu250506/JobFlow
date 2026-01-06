
<img width="1919" height="861" alt="Screenshot 2026-01-06 223925" src="https://github.com/user-attachments/assets/2dae8766-931c-4e4d-9ff7-f4d1dec72c84" />

<img width="1900" height="868" alt="Screenshot 2026-01-06 223954" src="https://github.com/user-attachments/assets/c0ccfe60-de0f-4567-ae4e-10d0a513318b" />

<img width="1901" height="864" alt="Screenshot 2026-01-06 224215" src="https://github.com/user-attachments/assets/55e88cf9-e387-4690-b8a2-95eee50860f7" />

<img width="1894" height="860" alt="Screenshot 2026-01-06 224232" src="https://github.com/user-attachments/assets/f0b1e644-6a2b-4244-97cb-e8e4e8b292af" />

<img width="1901" height="860" alt="Screenshot 2026-01-06 224250" src="https://github.com/user-attachments/assets/d3c9b99b-1190-4da6-8bb0-7f3587b6578b" />


<img width="1874" height="863" alt="Screenshot 2026-01-06 224307" src="https://github.com/user-attachments/assets/f58906cf-2bc1-4a20-aabd-492910c2a9bc" />

<img width="1890" height="875" alt="Screenshot 2026-01-06 224429" src="https://github.com/user-attachments/assets/f51c7bea-1c04-4a4c-9557-36594fb4fe14" />





Here is a professional and comprehensive README.md for your project JobFlow.

You can place this file in the root directory of your project (or separate ones for client/server if you prefer).

🚀 JobFlow - AI-Powered Job Application Assistant
JobFlow is a full-stack career acceleration platform designed to streamline the job search process. It leverages Google Gemini AI to audit resumes, generate tailored cover letters, and prepare users for interviews. The standout feature, Batch Apply, allows candidates to send personalized cold emails to multiple recruiters simultaneously with automatically attached resumes and portfolio links.

✨ Key Features
🤖 1. AI Career Architect
Resume Audit: detailed ATS compatibility scoring and keyword optimization suggestions.

Interview Prep: Generates role-specific technical and behavioral questions with model answers.

Cover Letter Generator: Creates custom cover letters based on specific job descriptions.

📧 2. Smart Batch Apply (Cold Emailing)
Bulk Outreach: Send personalized emails to multiple recruiters in one click.

Auto-Personalization: Dynamically replaces {role} and {company} in your email body.

Smart Attachments: Automatically appends your Resume link, LinkedIn, and Portfolio signature from your profile settings—no need to copy-paste every time.

Review Mode: Safety-first confirmation modal before blasting emails.

👤 3. Intelligent Profile & Resume Parser
PDF Parsing: Upload a resume to automatically extract skills, experience, and contact info.

Centralized Assets: Store your "Master Resume Link" and social profiles once; they are used everywhere across the app.

📊 4. Dashboard & History
Analytics: Track profile strength, applications sent, and AI usage.

Activity Log: View a history of every AI generation and email sent.

🛠️ Tech Stack
Frontend (Client)
Framework: React (Vite)

UI Library: Material UI (MUI) & Tailwind CSS (Utility classes)

Icons: Lucide React

State Management: Context API

Routing: React Router DOM

HTTP Client: Axios

Markdown: React Markdown (for AI responses)

Backend (Server)
Runtime: Node.js

Framework: Express.js

Database: MongoDB (Mongoose)

AI Engine: Google Gemini API (@google/generative-ai)

Email Service: Nodemailer (SMTP)

File Handling: Multer (Memory Storage)

Security: JWT Authentication, Express Rate Limit

🚀 Getting Started
Prerequisites
Node.js (v18+)

MongoDB (Local or Atlas)

Google Gemini API Key

SMTP Credentials (Gmail App Password or similar)

1. Clone the Repository
Bash

git clone https://github.com/your-username/jobflow.git
cd jobflow
2. Backend Setup
Bash

cd server
npm install
Create a .env file in the server directory:

Code snippet

PORT=5000
MONGO_URI=mongodb://localhost:27017/jobflow
JWT_SECRET=your_super_secret_key

# Google AI
GEMINI_API_KEY=your_gemini_api_key

# Email Service (Nodemailer)
EMAIL_HOST=smtp.gmail.com
EMAIL_PORT=465
EMAIL_SECURE=true
EMAIL_USER=your_email@gmail.com
EMAIL_PASS=your_app_password
Start the server:

Bash

npm run dev
3. Frontend Setup
Bash

cd ../client
npm install
Start the client:

Bash

npm run dev
📖 Usage Guide
Setting Up Your Profile (Crucial Step)
Go to the Profile page.

Tab 1 (Profile & CV): Upload your PDF resume to parse details or manually edit your skills and experience.

Tab 2 (Application Settings):

Resume Link: Paste a link to your resume (Google Drive/Dropbox/hosted PDF).

Links: Add your LinkedIn and Portfolio.

Default Email: Write your master template using {role} and {company} placeholders.

Click Save.

Using Batch Apply
Navigate to Batch Apply.

Your email body and subject will auto-load from your profile settings.

Add recipients (Company Name, Email, Role) in the table.

Click Review & Send.

The system will personalize each email and automatically append your professional signature with the links you saved in your profile.

Using AI Tools
Go to AI Tools.

Select Resume Audit and enter a target job title to check your ATS score.

Select Interview Prep to get practice questions for a specific role.

📂 Project Structure
jobflow/
├── client/                 # React Frontend
│   ├── src/
│   │   ├── components/     # Reusable UI components
│   │   ├── pages/          # Dashboard, Profile, BatchApply, etc.
│   │   ├── context/        # Auth Context
│   │   └── api/            # Axios instance
│
├── server/                 # Node.js Backend
│   ├── controllers/        # Logic for Profile, AI, Applications
│   ├── models/             # Mongoose Schemas (User, Profile, Application)
│   ├── routes/             # API Endpoints
│   ├── service/            # AI (Gemini) & Email (Nodemailer) logic
│   └── middleware/         # Auth & Rate Limiting
🤝 Contributing
Contributions are welcome! Please fork the repository and create a pull request for any feature updates.

