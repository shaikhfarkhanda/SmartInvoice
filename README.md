SmartInvoice

SmartInvoice is a secure and modern full-stack web application that allows users to create, manage, and send professional invoices. Built with Django and React, it provides authentication via JWT tokens, invoice filtering, PDF generation, and email functionality.

🚀 Features

✅ Authentication

  Secure JWT-based login/logout
  
  Auto token refresh
  
  Protected routes for logged-in users

✅ Invoice Management
  
  Add clients with name and email
  
  Add multiple line items (description, quantity, rate)
  
  Generate invoice numbers and calculate totals
  
  Add notes, issue dates, and due dates

✅ Invoice Listing

  List all invoices
  
  Filter by status: All, Paid, Unpaid
  
  View totals and status at a glance

✅ Invoice Details

  View full invoice details
  
  Mark invoices as Paid
  
  Download invoices as PDF
  
  Send invoices via email (PDF attached)

🧰 Tech Stack

  Layer
  
  Technologies
  
  Frontend
  
  React, TypeScript, Tailwind CSS, Vite, Axios
  
  Backend
  
  Django, Django REST Framework, SimpleJWT
  
  Database
  
  PostgreSQL (Render cloud database)
  
  PDF/Email
  
  WeasyPrint, Gmail SMTP
  
  Deployment
  
  Vercel (frontend) + Render (backend & DB)

🌐 Deployment

  Frontend hosted on Vercel
  
  Backend hosted on Render

  Environment variables managed securely

📁 Project Structure

    SmartInvoice/
    ├── backend/ (Django project)
    │   ├── invoices/ (App with models, views, serializers)
    │   ├── server/ (settings, urls, wsgi)
    │   └── requirements.txt
    ├── frontend/ (React app)
    │   ├── src/
    │   ├── public/
    │   └── vite.config.ts
    └── render.yaml

🔐 Environment Variables

  Backend (Render)
  
  DJANGO_SECRET_KEY
  
  DJANGO_ALLOWED_HOSTS
  
  DATABASE_URL (injected from Render DB)
  
  Frontend (Vercel)
  
  VITE_API_BASE_URL=https://your-backend-url.onrender.com

📦 How to Run Locally

  Backend
  
  cd backend
  pip install -r requirements.txt
  python manage.py runserver
  
  Frontend
  
  cd frontend
  npm install
  npm run dev

## 🚀 Live Demo

- **Frontend (React + Vite):** [smartinvoice-frontend.vercel.app](https://smart-invoice-frontend-gez2.vercel.app)
- **Backend API (Django + JWT):** [smartinvoice-backend.onrender.com](https://smartinvoice-backend.onrender.com)

- ## 🔐 Test Credentials

- **Username:** admin
- **Password:** admin123

📧 Contact

Created by Shaikh Farkhanda — feel free to reach out for questions or collaboration!

✨ This project showcases a complete professional-grade full-stack invoice system with real-world deployment and authentication best practices.

