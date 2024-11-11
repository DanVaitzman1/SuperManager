# SuperManager - Management System

## Project Overview
The **SuperLee Management System** is designed to digitize and automate the operations of a growing supermarket chain. It integrates modules for managing employees, inventory, suppliers, and logistics to streamline business processes and ensure efficient operations.

### Key Features:
- **Employee Management:** Shift scheduling, role assignment, and employee details management.
- **Inventory Management:** Real-time tracking of stock, notifications for low inventory, and defective item reporting.
- **Supplier Management:** Handling supplier contracts, purchase orders, and delivery scheduling.
- **Logistics Management:** Managing deliveries between suppliers and stores, with built-in safety measures for weight limits and driver compliance.

---

## Installation Instructions

1. **Prerequisites:**
   - Java Development Kit (JDK) version 17.0.1 or higher.
   - A relational database compatible with SQLite.
   - Libraries required for GUI development using SWING.

2. **Setup:**
   - Clone the repository or extract the downloaded `.zip` file:
     ```bash
     git clone <repository-url>
     cd SuperLee
     ```
   - Ensure the database is populated with sample data. The database file `superlee.db` is included in the `data` folder.

3. **Running the Application:**
   - To start the application in CLI mode:
     ```bash
     java -jar SuperLeeMainCLI.jar
     ```
   - To start the application in GUI mode:
     ```bash
     java -jar SuperLeeMainGUI.jar
     ```
   - You can also pass user roles as arguments to limit access:
     ```bash
     java -jar SuperLeeMainGUI.jar StoreManager
     ```

---

## Usage Guide

### Employee Management:
- **Adding Employees:** Access the "Add Employee" form from the main menu.
- **Shift Scheduling:** Use the "Schedule Shift" option to assign employees based on their availability.

### Inventory Management:
- **Restocking Notifications:** The system sends alerts when stock falls below a predefined minimum.
- **Viewing Inventory Reports:** Navigate to "Reports > Inventory" to view detailed reports on current stock levels and defective items.

### Supplier Management:
- **Creating Purchase Orders:** Select a supplier and items, then generate a purchase order from the "Supplier Management" menu.
- **Managing Supplier Contracts:** Update contract details directly from the "Edit Supplier" option.

### Logistics:
- **Planning Deliveries:** Schedule deliveries and track logistics using the "Logistics" module.
- **Weight Management:** Ensure truck weights comply with legal limits. The system will issue a warning if exceeded.

---

## Modules

1. **Employee Management:**
   - Tracks employee roles, availability, and shifts.
   - Enforces role-specific permissions for various tasks.

2. **Inventory Management:**
   - Monitors stock across multiple stores and warehouses.
   - Supports categorization by type, size, and supplier.

3. **Supplier Management:**
   - Handles supplier data, product catalogs, and discounts.
   - Automates recurring orders based on inventory needs.

4. **Logistics Management:**
   - Plans and records shipments between suppliers and stores.
   - Includes compliance checks for truck weights and driver licenses.

---

## Technical Details

- **Programming Language:** Java
- **Database:** SQLite
- **Libraries:**
  - **Swing** for GUI components.
  - Additional dependencies included in the `libs` folder.

---


## Notes

1. Ensure all diagrams (e.g., ERD, use case diagrams) are included in the `docs` folder.
2. Detailed error-handling procedures are implemented to prevent system crashes.
3. Sample data is provided for testing various scenarios.
