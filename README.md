# 🏥 MedLeave – Smart Medical Clinics Leave Management Platform

MedLeave is a modern HR web platform designed to **digitize and streamline medical leave management** for organizations.  
It replaces manual, paper-based workflows with a secure, role-based system that allows employees to submit medical leave requests and administrators to review, approve, and manage them efficiently — all in one place.

🌐 **Live Demo:**  
👉 https://medleave.lovable.app

---

## ❗ Problem Statement

Organizations often rely on email threads, spreadsheets, or paper forms to handle medical leave requests. This leads to:

- ❌ Poor tracking and visibility  
- ⏳ Delayed approvals  
- 📉 Inconsistent enforcement of HR policies  
- 🔒 Data loss and compliance risks  

---

## ✅ Solution Overview

MedLeave solves these challenges by providing:

- 📌 A centralized system for medical leave requests  
- 📜 Policy-aware validation (government & HR rules)  
- 👥 Clear role-based access control  
- 🔄 Real-time status tracking and historical records  

---

## 👤 User Roles

### 1️⃣ Employee
- Secure login
- Submit medical leave requests
- Upload medical documents
- Track request status (**Pending / Approved / Rejected**)
- View personal leave history

### 2️⃣ Admin (Manager Role)
- Elevated login privileges
- View all employee leave requests
- Approve or reject requests
- Add rejection notes
- Manage leave categories and rules
- View system-wide analytics and history

ℹ️ *There is no separate manager role — Admin handles all management responsibilities.*

---

## ⭐ Core Features

### 🔐 Authentication & Authorization
- Secure login via **Lovable Cloud Auth**
- Role-based access control (**Employee / Admin**)

### 📝 Medical Leave Management
- Medical leave request creation
- Automatic leave duration validation
- Medical document uploads
- Request lifecycle:
  - Pending
  - Approved
  - Rejected

### 📋 HR Policy Enforcement
- Government-aligned leave duration rules
- Validation before submission
- Prevents excessive or invalid leave requests

### 📊 Admin Dashboard
- View all requests
- Filter by status, employee, or date
- Approval & rejection workflows
- Audit-ready history

### 🧾 History & Tracking
- Employee leave history
- Admin decision logs
- Timestamped records

---

## 🧪 Prototype Scope

This prototype includes:

- 👥 2 users only  
  - 1 Admin  
  - 1 Employee  
- 🔄 Full end-to-end workflow:
  - Request submission → Review → Approval / Rejection  
- ✅ All core features fully implemented

---

## 🛠️ Tech Stack

### Frontend
- **Lovable** (AI-powered full-stack builder)
- Responsive, component-based UI

### Backend
- **Lovable Cloud** (Supabase-powered)
- PostgreSQL database
- Secure API layer

### Authentication
- Supabase Auth (via Lovable Cloud)

### Storage
- Supabase Storage (medical documents)

### Hosting
- Lovable Cloud  
- Public deployment: https://medleave.lovable.app

---

## 🗄️ Database Design (High Level)

### users
- id
- name
- email
- role (admin / employee)

### leave_requests
- id
- user_id
- leave_type
- start_date
- end_date
- duration
- status
- admin_note
- created_at

### documents
- id
- request_id
- file_url
- uploaded_at

---

## 🎨 Design Principles

- Simple and intuitive UX
- Clear separation of roles
- Policy-first validation
- Full auditability and traceability
- Scalable foundation for future HR modules

---

## 🔮 Future Enhancements

- Multi-center / multi-department support
- Email & notification system
- Annual leave & unpaid leave modules
- Exportable reports (PDF / Excel)
- Role hierarchy (HR, Manager, Admin)
- Mobile-first UI optimization

---

## 📸 Screenshots

> Capture screenshots directly from the live demo:  
> 👉 https://medleave.lovable.app  
>  
> Save images in a `/screenshots` folder and update the paths below.

### 🔑 Login Page
![Login Page](screenshots/login.png)

### 👨‍⚕️ Employee Dashboard
![Employee Dashboard](screenshots/employee-dashboard.png)

### 📝 Leave Request Form
![Leave Request Form](screenshots/leave-request-form.png)

### 🛡️ Admin Dashboard
![Admin Dashboard](screenshots/admin-dashboard.png)

### ✅ Approval Workflow
![Approval Workflow](screenshots/approval-workflow.png)

---

## ▶️ How to Run Locally (Optional)

This project is primarily hosted on **Lovable Cloud**.  
Local development depends on Lovable’s CLI and environment setup.

---

## 📄 License

This project is a **prototype** developed for demonstration and educational purposes.

---

## 👨‍💻 Author

**Nihad Alsufe**  
Tech Enthusiast & Software Engineer

---

⭐ If you find this project useful, consider giving it a star on GitHub!
