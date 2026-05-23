# Software Requirements Specification (SRS)
## BK Restaurant Management System

**Version:** 1.0 Draft  
**Date:** 22 May 2026  
**Prepared By:** SENG 31242 Team  

---

## 1. Introduction

### 1.1 Purpose and Scope
The purpose of this document is to outline the Software Requirements Specification for the BK Restaurant Management System. This system aims to digitize and centralize operations across three branches, replacing manual WhatsApp orders, physical books, and verbal communications with a unified digital platform. The scope includes Online Ordering, a Kitchen Display System (KDS), Delivery Tracking, Inventory Management, and Employee Management.

### 1.2 Definitions, Acronyms, Abbreviations
* **SRS**: Software Requirements Specification
* **KDS**: Kitchen Display System
* **POS**: Point of Sale
* **GPS**: Global Positioning System

### 1.3 Overview of Document
This document follows the standard SRS outline covering Overall Description, System Analysis (including Use Cases and Fact-Finding), Functional Requirements, and Non-Functional Requirements.

### 1.4 Problem Statement
The BK Restaurant currently operates across three distinct branches (including Ambalangoda and Kahawa) using entirely manual processes. Customer orders are received via ad-hoc WhatsApp messages and phone calls, leading to high error rates and missed orders. Internally, cashiers rely on verbal communication to relay orders to the kitchen, resulting in frequent preparation mistakes. Furthermore, there is zero visibility into delivery rider locations, and inventory is managed through disjointed physical books. This decentralized, manual approach completely deprives the restaurant owner of real-time oversight, causing operational bottlenecks, supply chain inefficiencies, and significant revenue leakage.

### 1.5 Project Goals
The primary goals of the BK Restaurant Management System are to:
1. **Digitize Order Workflows:** Replace WhatsApp/phone manual entry with a unified Point of Sale (POS) and automated Kitchen Display System (KDS).
2. **Centralize Oversight:** Provide a single, cloud-synced dashboard for the owner to monitor sales, attendance, and inventory across all branches simultaneously.
3. **Automate Delivery Tracking:** Implement a proprietary Rider App with live GPS tracking to ensure delivery accountability.
4. **Mitigate Stockouts:** Transition from physical inventory books to a real-time digital tracking system with automated low-stock alerts and direct digital supplier requests.

---

## 2. Overall Description

### 2.1 Product Perspective
The BK Restaurant Management System is a comprehensive, standalone system consisting of a web-based management dashboard, a POS interface for cashiers, a KDS for kitchen staff, an online ordering portal for customers, and a mobile application for delivery riders.

### 2.2 User Classes and Characteristics
* **Restaurant Owner**: Needs high-level visibility across all branches.
* **Branch Manager**: Needs localized control over inventory, employees, and daily operations.
* **Cashier**: Needs a fast POS system to input orders quickly.
* **Kitchen Staff**: Needs clear, readable digital tickets to prepare food without verbal miscommunications.
* **Delivery Rider**: Needs a mobile interface with GPS navigation to deliver orders.
* **Customer**: Needs an intuitive interface to place and track orders.

### 2.3 Operating Environment
* Web interfaces will run on modern web browsers (Chrome, Safari, Firefox).
* The KDS will run on tablets/screens in the kitchen.
* The Rider App will be compatible with Android and iOS.

---

## 3. System Analysis

### 3.1 Fact-Gathering Techniques Used
1. **Structured Interview**: Conducted with the Restaurant Owner (Mr. Sanjeewa De Silva) on 21/05/2026 to understand high-level pain points.
2. **Questionnaire/Survey**: Distributed to Branch Managers at Ambalangoda and Kahawa branches to gather data on localized operational bottlenecks.

### 3.2 Existing System Analysis (Pain Points)
* All orders and records are managed manually via WhatsApp and physical books.
* No centralized oversight for the owner across the three branches.
* Delivery riders cannot be tracked once they leave the premises.
* Verbal communication between cashiers and kitchen staff causes frequent order errors.
* Inventory shortages are only discovered when items run out mid-shift.

### 3.3 System Analysis Diagrams
* **Use Case Diagram**: `diagrams/exports/use_case_diagram.svg`
* **Activity Diagrams**: 
  - Place Online Order: `diagrams/exports/act-UC-01.svg`
  - Process Walk-in Order: `diagrams/exports/act-UC-03.svg`
  - View & Update Order (KDS): `diagrams/exports/act-UC-04.svg`
  - Update Delivery Status: `diagrams/exports/act-UC-05.svg`
  - Manage Inventory: `diagrams/exports/act-UC-06.svg`

*(Refer to the `diagrams/` directory and `use-cases/` directory for detailed descriptions).*

---

## 4. Functional Requirements

| ID | Title | Description | Priority |
| :--- | :--- | :--- | :--- |
| **FR-01** | Central Dashboard | The system shall provide a web-based dashboard allowing the owner to view real-time sales, inventory, and attendance across all branches. | P1 – Blocker |
| **FR-02** | POS Order Entry | The system shall allow cashiers to digitally input walk-in orders and print receipts. | P1 – Blocker |
| **FR-03** | Kitchen Display Sync | The system shall automatically send confirmed orders to the Kitchen Display System (KDS) without requiring manual verbal communication. | P1 – Blocker |
| **FR-04** | Rider GPS Tracking | The system shall track and display the live GPS location of delivery riders on the central dashboard while they are "Out for Delivery". | P2 – Critical |
| **FR-05** | Inventory Alerts | The system shall automatically generate low-stock alerts and notify the branch manager when stock levels fall below a predefined threshold. | P2 – Critical |
| **FR-06** | Digital Leave Management | The system shall allow employees to submit leave requests digitally for manager/owner approval. | P3 – Major |

---

## 5. Non-Functional Requirements

| Type | Requirement |
| :--- | :--- |
| **Performance** | The KDS must update within 2 seconds of the cashier confirming an order. |
| **Security** | Role-based access control (RBAC) must ensure that cashiers cannot access the inventory dashboard or modify stock levels. |
| **Usability** | The Rider mobile app must feature high-contrast UI elements to be readable outdoors in direct sunlight. |
| **Reliability** | The POS must have an offline-first capability, syncing data automatically when internet connectivity is restored. |

---

## 6. Alternative Solutions & Feasibility Study

### 6.1 Alternatives Analysed
1. **Off-the-shelf POS (e.g., Square or Toast)**: High recurring subscription fees and lacks customized multi-branch dashboard requirements specific to Sri Lankan operational flows.
2. **Custom Developed System**: Higher initial time investment but zero recurring subscription fees and 100% customizable to Mr. Sanjeewa's specific requirements.

### 6.2 Feasibility Recommendation
**Recommended Approach:** Custom Developed System.
* **Technical Feasibility**: The team possesses the required skills (React, Node.js, React Native) to build the proposed stack.
* **Economic Feasibility**: The client is willing to cover server costs, which are significantly lower than enterprise POS SaaS subscriptions.
* **Operational Feasibility**: The custom UI will be designed specifically around the existing workflow to minimize staff training time.
