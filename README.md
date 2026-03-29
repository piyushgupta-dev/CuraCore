# 🌿 Ayursutra — Panchakarma Management System

> **A modern digital solution for Panchakarma clinics** — streamlining therapy scheduling, patient records, inventory, and follow-up care while preserving the authenticity of Ayurveda.

---

## 📌 Project Metadata

- **Project Title**: Ayursutra — Panchakarma Management System
- **Team Name**: JM_Cura Core
- **Problem Statement ID**: SIH25023
- **Repository Link**: _[Add your repo link here]_

---

## 📝 Executive Summary

Panchakarma clinics face inefficiencies in scheduling, patient record management, inventory tracking, and follow-up care — leading to delays, errors, and poor patient experience.

**Ayursutra** solves this by providing a secure, digital platform that:

- 📅 Automates therapy scheduling
- 📋 Digitizes patient records & consent
- 💊 Manages inventory with alerts
- 🔔 Sends pre- & post-procedure reminders
- 📊 Enables real-time reporting & analytics

**Impact** → Reduced wait times ⏳ | Improved compliance ✅ | Safer record management 🔒

---

## 🎯 Goals & Objectives

**Primary Objectives:**

- Digitize Panchakarma patient records & therapy schedules.
- Provide therapist-friendly scheduling & session management.
- Ensure informed consent & outcome tracking.

**Secondary Objectives:**

- Inventory & medicine stock management.
- Billing & payment tracking.
- Analytics for treatment effectiveness.

---

## ✨ Features

- 📅 **Automated Therapy Scheduling** (patients & practitioners)
- 🔔 **Notifications & Reminders** (SMS/Email/WhatsApp)
- 🧾 **Digital Consent Capture** with timestamp & versioning
- 📊 **Reports & Analytics** (CSV/PDF exportable)
- 💊 **Inventory Tracking** with low-stock alerts
- 💳 **Billing & Invoicing**
- 👩‍⚕️ **Therapist Dashboard** (daily roster, session notes)
- 📱 **Mobile-friendly UI** for patients & therapists

---

## 🖥️ Technology Stack

- **Frontend**: React (Web) + React Native / Flutter (Mobile)
- **Backend**: Node.js + Express / Python FastAPI
- **Database**: PostgreSQL (primary), Redis (cache/queues)
- **Storage**: AWS S3 (images & documents)
- **Auth**: JWT + Refresh Tokens, Role-Based Access
- **Integrations**: SMS/WhatsApp Gateway, Payment Gateway, Google Calendar API
- **Deployment**: Docker + GitHub Actions (CI/CD), AWS/GCP/DigitalOcean

---

## 🏗️ System Architecture (High-level)

---

## 📂 Data Models

**patients**: id, name, dob, gender, phone, email, address, blood_group, known_allergies, medical_history, aadhaar_or_identifier, created_at  
**therapists**: id, name, qualifications, specializations, availability_slots, contact  
**therapy_plans**: id, patient_id, prescribed_by, sessions[], start_date, end_date, notes  
**sessions**: id, patient_id, therapist_id, therapy_type, date, start_time, end_time, notes, outcome, photos[], consent_version  
**inventory**: id, item_name, batch_no, qty_available, reorder_level, supplier  
**payments**: id, patient_id, amount, method, status, invoice_ref  
**consents**: id, patient_id, consent_text_version, signed_at, signer_name

---

## ⚡ API Endpoints (Examples)

- `POST /api/auth/login` — returns JWT
- `POST /api/patients` — create patient
- `GET /api/patients/{id}` — get patient profile
- `GET /api/therapists/{id}/available?date=` — check availability
- `POST /api/bookings` — create appointment
- `PATCH /api/sessions/{id}` — update session notes
- `GET /api/reports/weekly` — aggregated data

---

## 🖼️ UI / Wireframes

Screens to include:

- Home / Dashboard
- Book Appointment
- Patient Profile
- Therapist Dashboard
- Admin Dashboard
- Inventory Page
- Billing Page
- Reports Page
- Consent Capture UI

---

## 🔒 Security & Privacy

- Encrypt sensitive fields in DB & HTTPS everywhere
- Role-based access control + session expiry
- Digital consent with timestamp & versioning
- Audit trail for edits to medical records
- Periodic encrypted backups

---

## 🚀 Installation & Setup

### Clone repo

git clone <https://github.com/your-repo-link.git>
cd ayursutra

### Backend

cd backend
npm install
npm run dev # OR FastAPI: uvicorn main:app --reload

### Frontend

cd ../frontend
npm install
npm start

### Run with Docker

docker-compose up --build

## 🧪 Testing Plan

- ✅ Unit tests for API endpoints
- 🔄 Integration tests (booking, payment, consent)
- 🧑‍💻 E2E tests with Playwright / Cypress
- 📈 Load tests (k6) for peak booking

---

## 📊 KPI / Success Metrics

- ⏳ Reduce patient wait times by **50%**
- 📅 Improve scheduling accuracy by **40%**
- 📲 Reduce missed appointments by **30%**
- 👍 Achieve **90%+** patient satisfaction

---

## 🔮 Future Scope

- 🤖 AI/ML to predict therapy effectiveness
- 📡 IoT vitals monitoring
- 🏥 Insurance & govt health record sync
- ⛓️ Blockchain for immutable records
- 📹 Teleconsultation module

---

## 🏆 Competitive Advantage

- Ayurveda & Panchakarma **focused**
- Real-time progress visualization (graphs & milestones)
- Feedback loop to refine therapy schedules
- Mobile-first design for therapists

---

## 👥 Team & Contributions

- **Frontend Lead** → Patient & Therapist UI
- **Backend/API Lead** → Core APIs & Integrations
- **Database & DevOps** → Schema, Docker, AWS Deployment
- **QA & Testing** → Automated + Manual coverage
- **Docs & Research** → SIH compliance, PPTs, video scripts

---

## 📜 Compliance & Regulations

- Align with India’s **DPDP Act 2023**
- Follow **HIPAA-like principles** for patient confidentiality
- Digital consent handling with timestamps & versioning
- Daily encrypted backups & retention policies

---

## 📧 Contact

- 📩 Email: _[piyushgupta140206@gmail.com]_
- 🔗 LinkedIn / Portfolio: _[https://www.linkedin.com/in/piyush-gupta-0a568828b/]_
  hor

### Piyush Gupta
