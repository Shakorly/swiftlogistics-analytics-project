# SwiftLogistics Performance Analytics System: A Case Study

This repository documents the end-to-end design of a data analytics solution for a last-mile logistics company. The project follows a formal, phased methodology from business requirements gathering to BI dashboard design.

---

## Phase 1: Strategy & Initiation

### 1.1 Problem Statement & Opportunity Analysis

**The Business Problem:**
SwiftLogistics Inc. is a third-party logistics (3PL) provider whose core value proposition is a 48-hour delivery Service Level Agreement (SLA). The company is currently failing to meet this SLA on approximately 30% of its packages, resulting in direct financial penalties, customer churn, and escalating operational costs (especially fuel). The root cause is a lack of data visibility; the existing fragmented tracking systems do not allow for a holistic analysis of the delivery lifecycle, making it impossible to identify the root causes of delays or measure operational efficiency.

**The Opportunity:**
By centralizing and analyzing its operational data, SwiftLogistics has the opportunity to:
- **Increase Profitability:** By identifying and resolving the root causes of delays, the company can avoid SLA penalties and reduce customer churn.
- **Reduce Operational Costs:** By analyzing route performance and fuel consumption, the company can optimize delivery routes, leading to significant fuel savings and reduced driver overtime.
- **Improve Service Quality:** By creating a data-driven performance culture, the company can consistently meet its 48-hour SLA, strengthening its brand reputation and competitive advantage.

This project will build the foundational data platform required to seize these opportunities.

### 1.2 Stakeholder Requirements

The following requirements have been gathered from the key project stakeholders and are tracked in the `Opportunity Stakeholder Matrix`.

| Req No | Requirement Description | Stakeholder(s) | Business Justification |
| :--- | :--- | :--- | :--- |
| REQ-001 | The system must calculate the overall On-Time Delivery (OTD) percentage for all packages, filterable by date, route, and distribution center. | COO, Logistics Mgr | To measure overall company performance against the core 48-hour SLA. |
| REQ-002 | The system must track the time a package spends in each delivery stage (Processing, In-Transit, Out for Delivery) to identify bottlenecks. | Logistics Mgr | To understand *where* in the lifecycle delays are occurring so they can be fixed. |
| REQ-003 | The system must identify the routes with the highest and lowest on-time delivery rates. | Logistics Mgr | To enable data-driven route optimization and planning. |
| REQ-004 | The system must measure the performance of individual drivers based on their on-time delivery percentage and number of completed deliveries. | Logistics Mgr | To identify top performers and drivers who may require additional training. |
| REQ-005 | The system must track fuel consumption and cost against packages delivered to measure the cost-efficiency of each route and DC. | COO, Fin Director | To control rising operational costs and improve profitability. |
