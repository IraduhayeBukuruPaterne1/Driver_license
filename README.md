# 🇧🇮 Driver’s License Digital System – Capstone Project

##  Description

This project is a **full-stack prototype** for digitizing the driver’s license application and verification process in Burundi. It provides an accessible web interface for applicants to verify their identity via OTP or fingerprint (simulated), upload driving school certificates, and receive a QR-embedded digital license. Traffic officers and government agencies can use the backend for real-time license verification.

The goal is to **decentralize**, **streamline**, and **digitally secure** public services — starting with licensing.

---

## 🔗 GitHub Repository

👉 [Click here to view the project repository](https://github.com/IraduhayeBukuruPaterne1/Driver_license)

---

**How to Set Up the Environment**

### 1. **Prerequisites**
- Node.js v18+
- MongoDB Atlas (or a local MongoDB instance)
- Git
- Internet for OTP simulation (Twilio/Firebase can be integrated)

### 2. **Installation**

```bash
**Clone the repository**  
git clone https://github.com/IraduhayeBukuruPaterne1/Driver_license.git

# Navigate to the project folder
cd Driver_license

# Install dependencies
npm install

# Create a `.env` file and include necessary variables
# Example:
# MONGODB_URI=your_mongo_db_connection_string
# OTP_SECRET=your_secret_key

# Run the development server
npm run dev

3. Running the App
Open your browser and go to:
http://localhost:3000

🎨 Designs and Visuals
✅ Figma Mockups & Flow
Wireframes & Flowchart: APPLICATION_FLOW.md

Mockup Screenshots: /public/designs/

App Screenshots

![Capture d'écran 2025-06-10 221326](https://github.com/user-attachments/assets/007ee348-3153-461e-8c11-4d68523ebdd5)
![Capture d'écran 2025-06-10 221309](https://github.com/user-attachments/assets/b8db552e-ce7a-4486-8cdb-cf60d2a231ef)
![Capture d'écran 2025-06-10 221247](https://github.com/user-attachments/assets/7ca7744c-49ec-4a2e-884d-339a2d3acbe9)
![Capture d'écran 2025-06-10 221209](https://github.com/user-attachments/assets/a3377201-2482-44b0-839e-cb3de6d04ba1)

Project Structure

├── public/                     # Static files & assets
├── src/                       
│   ├── app/                   # Pages (Next.js routing)
│   ├── components/            # Reusable UI components
│   ├── contexts/              # State management contexts
│   └── utils/                 # Utility functions
├── database/                  # (Optional) DB logic if separated
├── .gitignore
├── package.json
├── tsconfig.json

 Frontend Highlights
Framework: Next.js with TypeScript

Features:

User-friendly form navigation (step-by-step)

Responsive layout using Tailwind CSS

QR code display on dashboard

Conditional routes (e.g., /dashboard for logged-in users)

 Frontend Highlights
Framework: Next.js with TypeScript

Features:

User-friendly form navigation (step-by-step)

Responsive layout using Tailwind CSS

QR code display on dashboard

Conditional routes (e.g., /dashboard for logged-in users)

 Backend Highlights
Database: MongoDB Atlas

API Routes (via Next.js):

/api/register: stores new applicants

/api/verify: simulates OTP verification

/api/license: returns user license with QR

Security:

JWT-like mock for session

Future plan: Firebase Auth or Twilio for real OTP

Data Schema:

// Example schema
User {
  id: ObjectId
  name: string
  nationalId: string
  phoneNumber: string
  otp: string
  licenseQRCode: string
  drivingCertificate: string
}

Deployment Plan
Current Status: Local testing on localhost:3000
Next Steps:

Deploy frontend & backend using Vercel (Next.js native)

Connect MongoDB Atlas securely

Integrate Firebase Auth or Twilio for OTP

Use Cloudinary or Firebase for driving certificate file uploads

Host a read-only version for government verification offices

**Demo Video** 


https://drive.google.com/file/d/1Fnx4LHPsirvpOgUCN_pRDhWVaVOm-EXJ/view?usp=sharing
