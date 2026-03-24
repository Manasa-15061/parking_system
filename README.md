# 🚗 Smart Parking System (India)

A full-stack web application to find, book, and pay for parking slots in real-time.

---

## 📌 Overview

This system helps users:
- Find nearby parking areas
- Check real-time slot availability
- Book slots instantly
- Make secure payments (UPI/Card)

---

## ✨ Features

- 🔐 Authentication (JWT-based Login/Register)
- 📍 Real-time parking availability
- 🅿️ Slot booking system
- 🚫 Double booking prevention
- 💳 Razorpay payment integration (UPI, Cards)
- 📊 User dashboard (bookings, history)
- 🛠️ Admin panel (manage slots & parking areas)

---

## 🧱 Tech Stack

### Frontend
- React.js

### Backend
- Node.js

### Databases

| Purpose | Technology |
|--------|-----------|
| Parking data (slots, status) | MongoDB |
| Payments & transactions | PostgreSQL |
| Real-time & caching | Redis |
| Search & filtering | Elasticsearch |

---

## 🗄️ Database Design

### MongoDB
- parking_areas
- parking_slots
- bookings

### PostgreSQL
- payments
- transactions
- invoices

### Redis
- slot locks
- live location cache

### Elasticsearch
- parking search index

---

## 💳 Payment Integration

- Razorpay (India)
- Supports:
  - UPI (GPay, PhonePe, Paytm)
  - Cards
  - Net Banking

---

## 🔄 System Flow

1. User searches location  
2. Nearby parking fetched  
3. Availability checked (Redis + MongoDB)  
4. Slot selected  
5. Payment initiated (Razorpay)  
6. Payment verified  
7. Booking confirmed  
8. Data stored in PostgreSQL  

---

## ⚙️ Setup Instructions

### 1. Clone Repository

```bash
git clone https://github.com/YOUR_USERNAME/parking_system.git
cd parking_system
