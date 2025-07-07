# 🧩 Core Functionalities – Airbnb Clone Backend

## 📘 Overview

This document outlines the **key backend modules and features** of the Airbnb Clone project. It is intended to serve as a reference for developers, reviewers, and stakeholders, highlighting the system’s architectural scope and functional requirements.

The visual diagram (included separately) maps out the major subsystems, their responsibilities, and how they interact. It provides a modular view of the backend design, ensuring that all essential components are logically organized and well-documented.

---

## 🛠️ Functional Modules

| Module                | Description |
|-----------------------|-------------|
| **User Management**   | Handles user registration, login, roles (guest, host, admin), and profile updates. |
| **Property Management** | Allows hosts to create, update, and manage property listings. Integrates with booking and review systems. |
| **Booking System**    | Manages guest bookings, date validations, cancellations, and booking statuses. |
| **Payment System**    | Processes payments associated with bookings. Supports multiple payment methods. |
| **Review System**     | Enables guests to submit ratings and comments on properties. |
| **Messaging System**  | Allows users to exchange messages (e.g., guest ↔ host) with timestamps. |
| **Notification System** | Sends alerts to users regarding key events like booking confirmations or new messages. |
| **Admin Dashboard**   | Provides admin users with capabilities to manage users, monitor bookings and payments, and oversee platform activity. |
| **Search & Filtering**| Supports property discovery using location, price, date availability, and review scores. Integrates closely with property and booking modules. |

---

## 🔄 Relationships Between Modules

- **Users ↔ Properties**: Hosts manage multiple properties.
- **Users ↔ Bookings**: Guests can create bookings.
- **Properties ↔ Bookings**: A property can have many bookings.
- **Bookings ↔ Payments**: One-to-one relationship; each booking can generate a payment.
- **Users ↔ Reviews ↔ Properties**: Guests review properties they’ve booked.
- **Users ↔ Messages**: Users can send and receive messages.
- **Notifications**: Triggered by changes in bookings, messages, and other user actions.
- **Search**: Retrieves and filters property listings based on user queries.

---

## 📌 Diagram Access

The **Core Functionalities Diagram** was created using [Draw.io](https://draw.io) and is available in the `/docs` folder.

- `airbnb_core_features.drawio` – Editable source file
- `airbnb_core_features.png` – Exported visual
- `airbnb_core_features.pdf` – Print-ready format

---

## 📎 Purpose

This module-based architecture supports **clean separation of concerns**, promotes **scalability**, and makes the backend easier to **extend, maintain, and secure**.

---

> For ERD relationships and use case diagrams, refer to the respective files in the `/docs` directory.
