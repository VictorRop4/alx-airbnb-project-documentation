# 📘 Use Case Documentation – Airbnb Clone Backend

## 🎯 Objective

This document provides a structured overview of how users interact with the Airbnb Clone backend system. It is based on the functional modules outlined in the Core Features and Functionality Diagram and visualized through a UML-style Use Case Diagram.

---

## 👤 Actors

| Actor   | Description |
|---------|-------------|
| **Guest** | A user who can browse listings, make bookings, submit payments, and leave reviews. |
| **Host**  | A registered user who lists properties and manages bookings and guest interactions. |
| **Admin** | System administrator with access to manage users, listings, bookings, and payments. |

---

## 🔄 Use Cases by Actor

### 🧑‍💼 Guest Use Cases
- Register an account
- Login / Logout
- Search for properties
- View property details
- Filter search results (location, price, amenities, etc.)
- Make a booking
- Cancel a booking
- Make a payment
- Leave a review
- Send and receive messages
- Receive notifications (booking status, payment confirmation)

### 🏠 Host Use Cases
- Login / Logout
- Add a property listing
- Edit or delete listings
- View bookings for owned properties
- Respond to guest reviews
- Receive payouts from confirmed bookings
- Communicate with guests (messaging)
- Receive notifications (new booking, cancellation)

### 🛡️ Admin Use Cases
- Login
- View all users
- Manage listings
- Monitor bookings
- View and audit payment transactions
- Access the admin dashboard

---

## 🧩 Use Case Relationships

| Use Case | Includes / Extends |
|----------|---------------------|
| Make Booking | Includes: Payment |
| Search Properties | Extends: Filter Properties |
| Add Listing | Extends: Upload Images |
| Leave Review | Extends: View Booking History |

---

## 🗂 Diagram File

The Use Case Diagram has been designed using [Draw.io](https://draw.io) and is available in the `/docs` directory.

- `airbnb_use_case_diagram.drawio` – Editable source file
- `airbnb_use_case_diagram.png` – Exported image
- `airbnb_use_case_diagram.pdf` – Printable format

---

## 📌 Purpose

This use case documentation ensures clear understanding of how different user roles interact with the system. It supports system design, role-based access control, and future development planning.

