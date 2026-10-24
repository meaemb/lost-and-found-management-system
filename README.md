# Lost and Found Management System

A web-based multi-organization lost and found management system designed to connect users with participating organizations and support the complete process of reporting, matching, ownership verification, and item return.

## Project Overview

The system is designed for environments such as shopping malls, cinemas, cafes, hotels, fitness centers, universities, and other organizations that handle lost and found items.

Instead of requiring users to search through multiple independent lost and found services, the proposed platform provides a unified environment where users can report lost items and participating organizations can register found items.

The system supports automated item matching based on item characteristics, location, and time. Potential matches are treated as suggestions and do not automatically establish ownership. Ownership is verified separately using private verification information before an item can be returned.

## Main Features

- Lost item reporting
- Found item registration
- Search and filtering
- Automated similarity-based item matching
- Ownership claim submission and verification
- Return process tracking
- User notifications
- Multi-organization support
- Role-based access control
- Organization employee and administrator functionality

## User Roles

The proposed system includes four main user roles:

- General User
- Organization Employee
- Organization Administrator
- Platform Administrator

## Technology Stack

### Frontend
- React

### Backend
- Node.js
- Express.js

The technology stack was selected after comparing alternative frontend and backend technologies based on project requirements, maintainability, development efficiency, and suitability for a web-based multi-organization system.

## Documentation

Project documentation is available in the `docs/` directory and includes:

- Project Proposal
- Evidence of Relevance
- Literature Review
- Existing Systems Comparison
- Technology Comparison
- Requirements Specification
- System Architecture and Diagrams
- User Interface Prototype
- Verification and Evaluation Plan

## System Design

The proposed architecture follows a web-based client-server model consisting of:

- React frontend
- Node.js and Express backend
- Authentication and role-based access control
- Item management
- Automated matching
- Ownership verification
- Return process tracking
- Notification management
- Organization management
- Persistent data storage

Architecture, use case, and entity-relationship diagrams are available in the project documentation.

## UI Prototype

A preliminary user interface prototype has been prepared for the first pre-defense stage. It demonstrates the proposed visual design and key user workflows, including:

- User Dashboard
- Lost Item Reporting
- Found Item Search

The current prototype represents a design draft and may be refined during subsequent development stages.

## Project Status

Current stage: **First Pre-Defense**

The repository currently contains the project analysis, requirements, architecture, interface prototype, and verification and evaluation planning materials. Implementation and further refinement will continue during subsequent stages of the diploma project.

## Team

Astana IT University  
Educational Program: Software Engineering

- Makhanbetiyar Begina Berikbolkyzy — SE-2427
- Amralina Kamila — SE-2427

Supervisor: Alua Bauyrzhanovna Myrzakerimova

## Repository Structure

```text
lost-and-found-management-system/
├── docs/
│   ├── Project Proposal
│   ├── Evidence of Relevance
│   ├── Literature Review
│   ├── Existing Systems Comparison
│   ├── Technology Comparison
│   ├── Requirements Specification
│   ├── System Architecture and Diagrams
│   ├── User Interface Prototype
│   ├── Verification and Evaluation Plan
│   └── Figures
└── README.md
```
