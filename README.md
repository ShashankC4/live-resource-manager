# 📍 Spotly - Real-time Resource Hub

**Spotly** is a high-performance, real-time resource management dashboard designed for modern co-working spaces and gyms. It allows users to view, book, and monitor the availability of desks, meeting rooms, or equipment in real-time without refreshing the page.

---

## 🚀 The Mission
In high-concurrency environments (like a busy office at 9:00 AM), race conditions lead to double-bookings. Spotly solves this using **database-level locking** and **WebSocket broadcasting**, ensuring a "Single Source of Truth" for resource availability.

## 🛠️ Tech Stack
- **Backend:** Laravel 12 (PHP 8.3+)
- **Frontend:** Vue 3 (Composition API)
- **Bridge:** Inertia.js (The Modern Monolith)
- **Styling:** Tailwind CSS
- **Real-time:** Laravel Reverb (WebSockets)
- **Database:** MySQL (with Pessimistic Locking)
- **Testing:** Pest PHP

## ✨ Key Features
- **Live Status Board:** Color-coded grid showing real-time availability (Green = Free, Red = Occupied).
- **Atomic Bookings:** Implements `lockForUpdate()` to prevent two users from booking the same slot at the exact same millisecond.
- **Instant Updates:** Uses WebSockets to push status changes to all connected clients instantly.
- **Conflict Prevention:** Logic-heavy backend to handle overlapping time-slots.

## 🏗️ Architecture Highlights (For Recruiters)
- **Concurrency Control:** Utilizes database transactions and pessimistic locking to ensure data integrity during high traffic.
- **Inertia 2.0:** Leverages "Always" props and partial reloading for a snappy, SPA-like experience while keeping backend logic in Laravel.
- **Service Pattern:** Decouples booking logic from Controllers to ensure high maintainability and testability.

## 📥 Getting Started

### Prerequisites
- PHP 8.3+ & Composer
- Node.js & NPM
- MySQL

### Installation
1. **Clone the repo:**
   ```bash
   git clone [https://github.com/YOUR_USERNAME/spotly.git](https://github.com/YOUR_USERNAME/spotly.git)
   cd spotly