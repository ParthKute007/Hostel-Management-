# Hostel Management System — Project Statement

##  Overview
Many hostels and educational institutions still rely on manual, paper-based methods to manage room allocations and student records. This traditional system causes several operational issues such as slow room searches, difficulty retrieving admission IDs, lack of real-time occupancy visibility, and accidental double-booking of students.

This project aims to digitalize the workflow using a simple Python-based desktop application that is lightweight, easy to use, and does not require a complex database.

---

##  Objective
To develop a **desktop-based Hostel Management System** using Python that streamlines room allocation, maintains accurate records, and provides secure access to student information.

---

##  Scope

###  In Scope
- Digital representation of hostel rooms with capacity tracking.
- Admin-only access (PIN: **3939**) to view all registered student IDs.
- Automated logic to prevent assigning students to full rooms.
- Local storage using a JSON file for persistence.
- Dynamic update of room occupancy on check-in and check-out.

###  Out of Scope
- Online payment integration.
- Cloud backup or multi-device synchronization.
- Multi-role authentication beyond a single admin PIN.

---

##  Target Users
1. **Hostel Wardens**  
   Need an instant view of room availability and a simple process for admitting or checking out students.

2. **Administrative Staff**  
   Require secure access to the list of Admission IDs for billing, record validation, and audits.

---

##  Key Features

### 1. Room Inventory Management  
- Add rooms with attributes such as capacity, type, and price.
- Real-time display of available and occupied beds.

### 2. Smart Admission System  
- Ensures a student cannot be assigned to a full room.
- Stores admission details in local JSON storage.

### 3. Secure Admin Lookup  
- PIN-protected view for accessing all Admission IDs.
- Prevents unauthorized access to sensitive data.

### 4. Persistent Storage (JSON)  
- All room and student data is saved locally in a JSON file.
- Automatically loaded when the application restarts.

### 5. Dynamic Occupancy Tracking  
- Check-ins and check-outs instantly update vacancy status.
- Prevents double booking and maintains accurate room counts.

---

##  Non-Functional Requirements
- Lightweight application with no dependency on external databases.
- Easy setup and usage for non-technical staff.
- Basic input validation for maintaining data correctness.

---

##  Deliverables
- Python source code for the Hostel Management System.
- JSON storage file (`hostel_data.json`).
- README with installation and usage instructions.
- This **statement.md** for documentation.

---

##  Success Indicators
- No occurrence of double-booking or inconsistent room status.
- Smooth retrieval of Admission IDs using admin PIN.
- Persistent data across sessions without manual effort.

---

## ✒️ Prepared For
Hostel Administration  
**Date:** November 2025  

