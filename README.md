# ParkSmart - Vehicle Parking System

A full-featured web-based vehicle parking management system built with Python (Flask), HTML/CSS, and SQLite.

## Features
- 🅿️ Smart slot management (3 floors × 10 slots each)
- 🚗 Vehicle entry with auto slot assignment
- 🚪 Vehicle exit with billing calculation
- 🎟️ Printable tickets & receipts
- 📊 Reports & analytics dashboard
- 🔍 Search & filter vehicle records

## Vehicle Types & Rates
| Type  | Rate      |
|-------|-----------|
| Car   | ₹30/hour  |
| Bike  | ₹15/hour  |
| Truck | ₹60/hour  |

## Setup & Run

1. Install dependencies:
   ```
   pip install flask
   ```

2. Run the application:
   ```
   python app.py
   ```

3. Open browser: http://localhost:5000

## Project Structure
```
parking_system/
├── app.py              ← Flask backend + SQLite logic
├── parking.db          ← Auto-created SQLite database
├── requirements.txt
└── templates/
    ├── base.html       ← Common layout & sidebar
    ├── index.html      ← Dashboard
    ├── entry.html      ← Vehicle entry form
    ├── ticket.html     ← Entry ticket
    ├── exit.html       ← Vehicle exit/search
    ├── receipt.html    ← Payment receipt
    ├── slots.html      ← Slot grid by floor
    ├── vehicles.html   ← All vehicles table
    └── reports.html    ← Analytics & charts
```

## Database Schema
- **slots** — 30 parking slots across 3 floors (car/bike/truck)
- **vehicles** — All vehicle records with entry/exit times
- **payments** — Payment records per transaction
