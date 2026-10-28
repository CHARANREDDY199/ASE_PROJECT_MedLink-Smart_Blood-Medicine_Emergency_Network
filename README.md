# MediLink – Smart Blood & Medicine Emergency Network


## 📌 Project Overview

MediLink is a centralized, web-based emergency healthcare discovery platform designed to eliminate life-threatening delays during the "golden hour" of emergency medical care. When critical surgical emergencies, road trauma, or acute medical conditions occur, patients and families often struggle to locate compatible blood units or rare medicines due to data silos and reliance on manual phone inquiries.

MediLink directly bridges this gap by connecting patients, verified blood donors, volunteer dispatchers, and local pharmacies in a unified real-time network featuring location-based proximity matching powered by the Google Maps API.

---

## 👥 Team & Academic Details

* Course Name: Adaptive Software Engineering (ASE)
* Course Code: 24CI3201
* Academic Year: 2026–2027
* Project Guide: Bhavya Varma K

### Team Members

| S. No. | Name | Roll Number | Role / Module |
| :---: | :--- | :---: | :--- |
| 1 | A. Anil | 2420030130 | Emergency Blood Requests & Request Lifecycle Tracking |
| 2 | N. Girish Reddy | 2420030125 | User Authentication, Donor Profiles & Availability Engine |
| 3 | S. Sri Charan Reddy | 2420030127 | Medicine Finder, Pharmacy Services & Maps Integration |

---

## 🚀 Key Features

* Real-Time Blood Request Management: Create emergency blood requests with blood group, units required, hospital location, and urgency status.
* Proximity Donor Matching: Search and filter compatible donors by blood group and proximity using location coordinates.
* Medicine Finder: Instant search for essential medicines, stock availability, and 24/7 operating hours across verified pharmacies.
* Volunteer Response Network: Enable community volunteers to coordinate donor dispatch and transport logistics.
* Live Status Tracking: Real-time request state transitions (Open → Accepted → In-Progress → Completed).
* Interactive Geo-Mapping: Embedded Google Maps API to visualize routes and calculate shortest transit times.

---

## 🛠 Technology Stack

| Layer | Technology |
| :--- | :--- |
| Frontend | JSP (JavaServer Pages), HTML5, CSS3, JavaScript (ES6+), Bootstrap 5 |
| Backend | Java (Servlets, MVC Architecture) |
| Database | MySQL 8.0 |
| Database Connectivity| JDBC (Java Database Connectivity) |
| Application Server | Apache Tomcat 9.0 / 10.0 |
| External APIs | Google Maps JavaScript API, Places API, REST Web Services |
| Version Control & PM | Git, GitHub, Jira (Agile Scrum) |

---

## 🏗 System Architecture

               Patient / Hospital Staff / Donor
                              │
                              ▼
                 ┌──────────────────────────┐
                 │  Presentation Tier (UI)  │
                 │   JSP, HTML5, CSS3, JS   │
                 └────────────┬─────────────┘
                              │ HTTP Requests
                              ▼
                 ┌──────────────────────────┐
                 │    Controller Tier       │
                 │   Java Servlets / MVC    │
                 └────────────┬─────────────┘
                              │
            ┌─────────────────┴─────────────────┐
            ▼                                   ▼
┌───────────────────────┐           ┌───────────────────────┐
│     Business Layer    │           │   External Services   │
│  - Donor Matching     │           │  - Google Maps API    │
│  - Emergency Dispatch │           │  - Geocoding API      │
│  - Medicine Search    │           │  - Notification Bus   │
└───────────┬───────────┘           └───────────────────────┘
            │
            ▼
┌───────────────────────┐
│      Data Access      │
│      JDBC Driver      │
└───────────┬───────────┘
            │
            ▼
┌───────────────────────┐
│    MySQL Database     │
│   (Users, Inventory,  │
│    Requests, Donors)  │
└───────────────────────┘

---

## 🔄 Emergency Blood Request Lifecycle
