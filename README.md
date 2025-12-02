# Branch Location Manager (PoC)
### Software Engineering Internship | Fastenal India (Jan 2022 - May 2022)

![Angular](https://img.shields.io/badge/Frontend-Angular%2013-red) ![.NET](https://img.shields.io/badge/Backend-.NET%205-purple) ![MongoDB](https://img.shields.io/badge/Database-MongoDB-green) ![Status](https://img.shields.io/badge/Status-Deployed-success)

## 📖 Project Overview
This repository contains the documentation and architectural design for the **Branch Location Manager**, a full-stack Proof of Concept (PoC) developed during my final semester internship. The application was designed to solve the business need for visualizing and managing branch location data for internal stakeholders.

> **Note on Confidentiality:** Due to Non-Disclosure Agreements (NDA), the source code for this enterprise application cannot be shared publicly. This repository hosts the **System Design Documentation, Architecture Diagrams, and Methodology Reports** to demonstrate the engineering rigor applied during development.

---

## 🛠️ Technical Architecture

### 1. Frontend (Angular 13)
* **Component Design:** Modular architecture using Angular Material for a consistent enterprise UX.
* **Map Integration:** Utilized `angular-google-maps` to render geospatial data of branch locations, including interactive markers and info-windows.
* **State Management:** Implemented Route Guards (`AuthGuard`) to protect administrative dashboards.

### 2. Backend (.NET 5)
* **RESTful API:** Designed a secure API layer to handle authentication, data retrieval, and user management.
* **Security:** Implemented **AES Encryption** for sensitive data at rest and **Caesar Cipher** for lightweight obfuscation during transit (as per project requirements).
* **Endpoints:**
    * `POST /User/Auth` - Secure Login/Validation
    * `GET /Branch` - Retrieve location data with server-side pagination.

### 3. Database (MongoDB)
* **Schema Design:** Utilized a NoSQL document structure to handle flexible branch metadata.
* **Optimization:** Implemented **Server-Side Pagination** to handle large datasets efficiently, reducing network load by loading data in chunks rather than full table scans.

---

## 📐 System Design & UML

### Process Flow
The application follows a secure authentication flow before granting access to the geospatial dashboard.

![Process Flow Diagram](https://github.com/gshyam-diff/Fastenal_Internship/blob/main/Process%20Flow%20Diagram.png)
*(Refer to Chapter 3.2 in the attached report for the full sequence diagram)*

### Security Implementation
The system implements a dual-layer encryption strategy for user credentials.
* **Client-Side:** Basic obfuscation before transmission.
* **Server-Side:** Industry-standard **AES Encryption** before database storage.

---

## 📂 Repository Contents
* `Fastenal_Content.pdf`: The complete **Technical Report**, including High-Level Design (HLD), Low-Level Design (LLD), API Contracts, and Database Schema.
* UML Sequence Diagrams and Architecture Block Diagrams.

---

## 🚀 Key Achievements
* **Performance:** Reduced data load times by implementing **Server-Side Pagination** for the branch list view.
* **UX/UI:** Delivered a responsive dashboard allowing users to toggle between "List View" and "Map View" for spatial awareness.
* **Outcome:** The success of this PoC directly resulted in a **full-time employment offer** to join the Master Data Management team.

---
*Authored by Ghanashyam R K P*
*Intern -> Software Engineer | Fastenal India*
