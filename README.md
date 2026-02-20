# Allocator - Resource Management System

A real-time dashboard for managing and booking shared resources like desks or meeting rooms.

## Tech Stack
- **Backend:** Laravel 12
- **Frontend:** Vue 3 (Composition API)
- **Bridge:** Inertia.js
- **Real-time:** Laravel Reverb (WebSockets)
- **Database:** MySQL
- **Testing:** Pest PHP

## Key Functionality
- **Real-time Availability:** A grid view showing current resource status.
- **Concurrency Handling:** Using database-level locking to prevent double-bookings.
- **WebSocket Updates:** Instant status changes across all clients.

## Installation

1. **Clone the repo:**
   ```bash
   git clone [https://github.com/YOUR_USERNAME/allocator.git](https://github.com/YOUR_USERNAME/allocator.git)
   cd allocator