# Threat Modeling-101
#### An essential approach towards threat modeling a web application.

This document outlines the threat model for a standard web application architecture within our fintech company. The model identifies assets, threats, vulnerabilities, and the corresponding security controls.

## Architecture Components

- **Frontend** (Client-side)
- **Backend** (Server-side)
- **Database**
- **API Endpoints**
- **External Integrations** (payment gateways, email services)
- **Infrastructure** (servers, containers)
- **User Data and Authentication Mechanisms**
- **Admin Interface**

## Threat Modeling Steps

### 1. Identify Assets

- **User Data:** Personal Identifiable Information (PII), payment information, transaction data.
- **Application Data:** Source code, application configuration.
- **System Data:** Server configurations, network configurations, encryption keys.
- **Data in Transit:** API calls, data exchange between services.
- **Data at Rest:** Databases, backups.

### 2. Define Trust Boundaries

- Between user devices and the front end.
- Between the front end and the backend.
- Between the backend and the database.
- Between the application and external integrations.

### 3. Identify Potential Threats

- **Spoofing Identity:** Unauthorized access through stolen credentials.
- **Tampering:** Modifying data in transit or at rest.
- **Repudiation:** Performing illegal operations without traceability.
- **Information Disclosure:** Unauthorized access to sensitive data.
- **Denial of Service (DoS):** Overloading servers to disrupt service.
- **Elevation of Privilege:** Exploiting vulnerabilities to gain higher access.

### 4. Identify Vulnerabilities

- Insecure APIs.
- Weak authentication mechanisms.
- Insufficient logging and monitoring.
- Misconfigurations in servers or databases.
- Outdated software components.
- Insecure direct object references.

### 5. Model Threat Agents

- **External attackers:** Hackers, rival companies.
- **Insider threats:** Disgruntled employees.
- **Third-party service providers.**
- **Automated bots or scripts.**

### 6. Define Security Controls

- **Preventive Controls:** Firewalls, intrusion prevention systems, strict access controls, input validation.
- **Detective Controls:** Log analysis, intrusion detection systems.
- **Corrective Controls:** Incident response team, backup and restore procedures.
- **Deterrent Controls:** Security training, policy enforcement.

### 7. Prioritize Risks

- Risks are prioritized based on likelihood and impact. Focus on the ones that could cause the most damage or are the most likely to occur.

### 8. Document Everything

- A detailed report includes all the findings and proposed mitigation strategies.

### 9. Review and Revise

- Regularly update the threat model to adapt to new threats, vulnerabilities, and changes in the architecture.
