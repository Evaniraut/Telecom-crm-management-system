# Telecom CRM & Management System

A web-based **enterprise CRM and document management system** built to digitize SIP customer records, streamline application workflows, automate administrative document generation, and manage customer information through a centralized platform.

## Overview

The system replaces manual, paper-based workflows with a searchable digital platform for managing customer applications, SIP details, scanned documents, estimates, administrative letters, and user activities.

It is designed for professional and operational use, with a focus on structured information management, role-based access, usability, and workflow efficiency.

## Features

### Customer & CRM Management

* Digital customer registration and application workflows
* SIP customer record management
* Enterprise broadband and telecom customer information
* Application status tracking
* Search and filtering by customer, file number, and SIP details

### Document Management

* Digitization of physical customer records
* Upload and management of scanned documents
* Linking documents to customer and SIP records
* Centralized searchable document archive

### Automated Estimates & Documents

* Automatic calculation of Non-Recurring Charges (NRC)
* Automatic calculation of Monthly Recurring Charges (MRC)
* VAT calculation
* Generation of cost estimates
* Generation of formal administrative letters
* Printable and downloadable PDF/HTML documents

### Role-Based Access Control

* Separate Admin and User roles
* Granular permission system
* Restricted access to administrative functionality
* Secure authentication and password handling

Example permissions:

```text
view_logs
upload_docs
update_sip_docs
view_client_apps
manage_users
```

### Activity & Audit Logging

* Tracks user operations within the application
* Records actions with timestamps
* Logs activities such as viewing, editing, and updating records
* Provides administrative visibility into system usage

## UI / UX

The application follows an **enterprise-style UI** designed for professional workflows.

The interface focuses on:

* Clear information hierarchy
* Structured layouts
* Practical navigation
* Efficient data entry
* Readable tables and forms
* Consistent presentation
* Easy access to complex information

The design prioritizes usability and operational efficiency rather than unnecessary visual decoration.

## Technology Stack

| Technology           | Purpose                       |
| -------------------- | ----------------------------- |
| PHP 8.x              | Backend and application logic |
| MySQL / MariaDB      | Relational database           |
| HTML5                | Frontend structure            |
| CSS3                 | Styling and layout            |
| JavaScript           | Client-side functionality     |
| Apache               | Web server                    |
| XAMPP / WAMP         | Development environment       |
| PHPMailer            | Email functionality           |
| Web-to-PDF Print API | PDF generation                |

## Database Architecture

The system uses a relational MySQL/MariaDB database containing interconnected tables for users, customer applications, SIP records, documents, and activity logs.

### Core Tables

```text
users
admins
applications
sip_customers
scanned_docs
dashboard_companies
uploaded_files
user_activities
activity_logs
```

### Data Management

* Primary and foreign key relationships
* Structured relational data
* `utf8mb4` character encoding
* JOIN-based data retrieval
* Search and filtering functionality
* Separation of user, customer, document, and activity data

## System Architecture

```text
Users / Workstations
        │
        ▼
   Web Browser
        │
        ▼
 Apache Web Server
        │
        ▼
  PHP Application
        │
        ▼
 MySQL / MariaDB
```

## Network Deployment

The application can be hosted on an Apache server within a local area network (LAN), allowing multiple authorized workstations to access the system through the internal network.

The deployment involves:

* Apache server configuration
* PHP environment setup
* Database configuration
* Local network access
* File and directory permissions
* Multi-user access through local IP routing

## Security

The system incorporates several security and access-control mechanisms:

* Role-based access control
* Granular permissions
* Password hashing
* Restricted administrative functionality
* User activity logging
* Controlled access to customer documents

## Challenges Addressed

### Interconnected Application Logic

Debugged and isolated issues across PHP modules by separating backend database operations from frontend form workflows.

### Bulk Record Digitization

Implemented verification and filtering workflows to improve the accuracy of digitized SIP records when transferring information from physical documents.

### Multi-User LAN Access

Configured server paths, directory permissions, and database connections to support access from multiple computers within the local network.

## Objectives

* Digitize paper-based customer records
* Centralize SIP and customer information
* Improve document accessibility
* Reduce repetitive administrative work
* Automate estimate and document generation
* Provide controlled access to sensitive information
* Maintain an auditable history of system activity

## Project Status

**Completed**

> This repository is intended for demonstration and portfolio purposes. Confidential information and real customer data have been excluded.
