# Initial Requirement Identification
## BK Restaurant Management System

Based on stakeholder discussions, interview findings, literature review findings, and the proposed system presentation, the following initial high-level requirements were identified for the BK Restaurant Management System. The identified requirements mainly focus on improving restaurant operations by reducing manual work, improving order management, supporting delivery coordination, and maintaining centralized business records across all branches.

---

## 1. Functional Requirements (FR)

### 1.1 User Management

- The system shall allow authorized users to securely log into the system.
- The system shall support role-based access for:
  - Restaurant Owner
  - Employees/Cashiers
  - Delivery Riders
  - Suppliers
- Users shall access system functions according to their assigned roles.

### 1.2 Order Management

- The system shall allow employees to create and manage customer orders.
- The system shall support dine-in, takeaway, and delivery orders.
- The system shall update order status in real time.
- The system shall allow order modifications and cancellations.
- The system shall generate digital bills and invoices.
- The system shall maintain customer order history records.

### 1.3 Delivery Management

- The system shall assign delivery orders to delivery riders.
- Delivery riders shall update delivery status through the mobile application.
- The restaurant owner shall monitor delivery progress in real time.
- The system shall provide estimated delivery times using GPS/location services.

### 1.4 Inventory Management

- The system shall maintain inventory records for all restaurant branches.
- Inventory shall automatically update after each sale.
- The system shall generate low-stock alerts.
- The system shall maintain supplier information and stock request records.
- The system shall support real-time inventory tracking.

### 1.5 Multi-Branch Management

- The system shall provide centralized monitoring for all restaurant branches.
- The restaurant owner shall view branch sales and operational reports.
- The system shall compare branch performance and revenue data.
- The system shall maintain branch-specific records.

### 1.6 Employee Management

- The system shall maintain employee information records.
- The system shall record employee attendance.
- The system shall support employee shift and schedule management.

### 1.7 Reporting and Analytics

- The system shall generate sales reports.
- The system shall generate inventory reports.
- The system shall generate delivery performance reports.
- The system shall provide dashboard-based analytics for business monitoring and decision-making.

---

## 2. Non-Functional Requirements (NFR)

### 2.1 Performance Requirements

- The system shall respond to user requests within an acceptable response time.
- The system shall support multiple users simultaneously.
- The system shall efficiently handle real-time order and delivery updates.

### 2.2 Security Requirements

- The system shall implement user authentication and authorization.
- The system shall protect business data from unauthorized access.
- The system shall securely store and back up system data.

### 2.3 Usability Requirements

- The system interface shall be user-friendly and easy to navigate.
- The system shall support simple workflows for non-technical users.
- The rider mobile application shall provide an easy-to-use interface.

### 2.4 Reliability Requirements

- The system shall maintain accurate and consistent records.
- The system shall minimize data loss during failures.
- The system shall provide stable operation with minimal downtime.

### 2.5 Scalability Requirements

- The system shall support future restaurant branch expansion.
- The system shall support increasing numbers of users and orders.

### 2.6 Maintainability Requirements

- The system shall be modular and easy to maintain.
- The system shall support future system enhancements and updates.

### 2.7 Compatibility Requirements

- The web application shall support modern web browsers.
- The mobile application shall support Android devices.
- The system shall integrate with GPS and map services.

---

## 3. Requirement Categories

| Category | Included Requirements |
|---|---|
| User Management | Authentication, role-based access |
| Order Management | Order handling, billing, order tracking |
| Delivery Management | Rider assignment, delivery monitoring, GPS tracking |
| Inventory Management | Stock updates, supplier management, low-stock alerts |
| Employee Management | Attendance, employee records, shift management |
| Reporting & Analytics | Dashboards, sales reports, branch performance |
| System Quality | Security, usability, performance, scalability |
