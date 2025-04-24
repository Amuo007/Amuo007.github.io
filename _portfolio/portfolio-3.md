---
title: "Waterloo - Academic Forms Management System"
excerpt: "A comprehensive Django web application designed for educational institutions to manage academic forms, approvals, and user authentication. This project implements a multi-department approval workflow system with role-based access control using Microsoft authentication.<br/><br/>The system manages various academic documents including Special Circumstance Forms, Course Drop Forms, FERPA Authorizations, and Texas Residency Affidavits. Forms progress through a customizable approval workflow involving different departments based on configurable business rules.<br/><br/>Key features include:<br/>• Microsoft OAuth integration for secure authentication<br/>• Role-based permissions (superuser, manager, approver, basic user)<br/>• Multi-department approval workflows<br/>• LaTeX-powered PDF generation<br/>• Digital signature management<br/>• External API integration for cross-system form submissions<br/>• Responsive Bootstrap UI with form validation<br/><br/>Technologies used:<br/>• Django 5.1<br/>• Microsoft Authentication Library (MSAL)<br/>• Bootstrap 5<br/>• LaTeX (pdflatex) for document generation<br/>• Docker/Docker Compose for containerization<br/>• SQLite/PostgreSQL databases<br/><br/>This project demonstrates my expertise in designing complex business workflow systems, implementing secure authentication, and creating intuitive user experiences for administrative applications.<br/><br/><br/><img src='https://amuo007.github.io//images/1.png'><br/><img src='https://amuo007.github.io//images/3.png'>"
collection: portfolio
---

## Overview
Waterloo is a Django-based web application designed to streamline the management of academic forms and their approval workflows for educational institutions. The system supports various document types with complex multi-department approval routing.

[View on GitHub](https://github.com/Amuo007/COSC-4353-Group-Project/tree/main)

## Technical Architecture

### Core Components
- **Django Backend**: Built on Django 5.1 with a modular approach using multiple apps
- **Authentication**: Microsoft OAuth integration using MSAL for secure, enterprise-ready login
- **Frontend**: Responsive Bootstrap 5 UI with form validation and AJAX functionality
- **Document Generation**: LaTeX templates with dynamic content insertion for professional PDFs
- **Database**: Flexible configuration supporting both SQLite and PostgreSQL
- **Containerization**: Docker and Docker Compose setup for consistent deployment

### Key Features

#### Role-Based Access Control
- **Superuser**: Complete system access with user and approval rule management
- **Manager**: Department-specific application approvals and user management
- **Approver**: Limited approval capabilities within assigned departments
- **Basic User**: Form submission with personal application tracking

#### Multi-Department Approval Workflow
- Configurable approval rules determine required departments for each form type
- Sequential or parallel approval patterns
- Comment system for returned forms requiring revision
- Approval tracking dashboard with notification system

#### Form Management
- Support for multiple form types:
  - Special Circumstance Forms
  - Course Drop Forms
  - FERPA Authorizations
  - Texas Residency Affidavits
- Draft saving and revision capabilities
- Digital signature upload and management
- Form status tracking (Draft, Pending, Approved, Returned)

#### PDF Generation
- Professional document generation using LaTeX templates
- Dynamic content insertion based on form data
- Signature embedding in generated documents
- Downloadable PDFs for record-keeping

#### External System Integration
- RESTful API for cross-system form submissions
- Integration with external form services
- Data validation and synchronization

## Development Challenges & Solutions

### Authentication & Security
Implemented Microsoft OAuth for enterprise-ready authentication while maintaining a secure session management system. Role-based permissions ensure users can only access appropriate system features.

### Approval Workflow Management
Designed a flexible system where administrators can define department approval requirements for each form type. The system tracks which departments have approved and requires appropriate permissions for approvals.

### PDF Generation
Integration of LaTeX for high-quality PDF generation required careful handling of user inputs, template management, and proper character escaping. The system generates professional-looking documents with embedded signatures.

### User Experience
Created an intuitive interface that guides users through form submission and approval processes with clear status indicators, validation, and helpful error messages.

## Demo Video
<div style="position:relative;padding-bottom:56.25%;height:0;overflow:hidden;">
  <iframe 
    src="https://www.youtube.com/embed/vOjlviS9_8c" 
    frameborder="0" 
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
    allowfullscreen 
    style="position:absolute;top:0;left:0;width:100%;height:100%;">
  </iframe>
</div>

## Screenshots
![Dashboard Screenshot](https://amuo007.github.io//images/1.png)


![Application List](https://amuo007.github.io//images/3.png)
