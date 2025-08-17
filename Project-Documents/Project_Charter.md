# Project Charter: SwiftLogistics Performance Analytics System

## 1. Project Mission & Vision

**Mission Statement:** To deliver a centralized data analytics platform that provides a single source of truth for all last-mile delivery operations.

**Vision:** To transform SwiftLogistics from a reactive to a proactive organization by embedding data-driven decision-making into its core operational and financial management processes.

---

## 2. Business Objectives & Success Criteria

This project is being initiated to achieve the following specific, measurable business goals. The project will be deemed successful when these criteria are met.

| Objective | Key Metric | Target |
| :--- | :--- | :--- |
| **Improve SLA Compliance** | On-Time Delivery (OTD) Percentage | Increase from 70% to >95% within 6 months of Go-Live. |
| **Reduce Operational Costs** | Average Fuel Cost Per Delivery | Decrease by 15% within 6 months of Go-Live. |
| **Increase Operational Visibility** | Reporting Lag Time | Reduce from weekly/manual to daily/automated. |
| **Enhance Performance Management**| Data-Driven Driver Reviews | Implement for 100% of drivers by year-end. |

---

## 3. Scope

### 3.1 In-Scope

- **Data Sources:** The project will exclusively use data from SwiftLogistics' internal package tracking and vehicle telematics systems.
- **Business Processes:** The scope is limited to the following processes:
    - Package lifecycle tracking (from DC receipt to final delivery).
    - Driver and vehicle performance monitoring.
    - Fuel consumption analysis.
- **Deliverables:**
    - A cloud-based Data Warehouse with a Kimball-style star schema.
    - An automated nightly ETL pipeline.
    - An interactive Power BI / Tableau dashboard for the key stakeholders.

### 3.2 Out-of-Scope

- **Real-time Driver Routing:** This project will provide the *analysis* to inform better routes, but it will **not** build a real-time, GPS-based re-routing application for drivers.
- **Warehouse Inventory Management:** The scope begins when a package is marked "Received at DC" and ends at final delivery. It does not include the management of retailer inventory within the DC.
- **Financial Accounting:** The system will analyze fuel costs but will not integrate with the company's general ledger or accounting software.

---

## 4. Key Stakeholders (RACI Matrix)

| Role | RACI |
| :--- | :--- |
| Chief Operations Officer (COO) | **A**ccountable |
| Logistics Manager | **R**esponsible, **C**onsulted |
| Finance Director | **C**onsulted, **I**nformed |
| IT Department | **C**onsulted |
| Drivers | **I**nformed |

---

## 5. Assumptions & Constraints

- **Assumptions:** Source system data is assumed to be available and reasonably accurate.
- **Constraints:** The initial solution must be built using the company's existing cloud provider and BI tool licenses.
