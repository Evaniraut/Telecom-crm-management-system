# Telecom CRM & Management System

A web-based enterprise CRM and document management system built to digitize SIP customer records, streamline application workflows, automate document generation, and manage customer information through a centralized platform.

## Overview

The system replaces manual, paper-based workflows with a searchable digital platform for managing customer applications, SIP details, scanned documents, estimates, administrative letters, and user activities.

It focuses on structured information management, role-based access, usability, and workflow efficiency.

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
* Generation of administrative letters
* Printable and downloadable PDF/HTML documents

### Role-Based Access Control

* Admin and User roles
* Granular permission system
* Restricted administrative functionality
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
* Logs viewing, editing, and updating activities
* Provides administrative visibility into system usage

## UI / UX

The application uses an enterprise-style interface designed for professional and operational workflows.

The interface focuses on:

* Clear information hierarchy
* Structured layouts
* Practical navigation
* Efficient data entry
* Readable tables and forms
* Consistent presentation
* Easy access to complex information

## Technology Stack

* PHP 8.x
* MySQL / MariaDB
* HTML5
* CSS3
* JavaScript
* Apache
* XAMPP / WAMP
* PHPMailer
* Web-to-PDF Print API

## Database

The system uses a relational MySQL/MariaDB database with interconnected tables for users, applications, customer information, documents, and activity logs.

Main tables:

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

## System Architecture

```text
Users / Workstations
        |
        v
   Web Browser
        |
        v
 Apache Web Server
        |
        v
  PHP Application
        |
        v
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

* Role-based access control
* Granular permissions
* Password hashing
* Restricted administrative functionality
* User activity logging
* Controlled access to customer documents

## Challenges

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

Completed

> This repository is intended for demonstration and portfolio purposes. Confidential information and real customer data have been excluded.

