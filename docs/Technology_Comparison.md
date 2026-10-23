# 5. Technology Comparison

## 5.1. Introduction

The selection of appropriate technologies is an important part of the development of the proposed Multi-Organization Lost and Found Management System. The selected technology stack should support the functional requirements of the system while remaining suitable for implementation within the scope of the project.

The system requires an interactive web interface for general users, organization employees, organization administrators, and the platform administrator. It also requires backend services for authentication, role-based access control, lost and found item management, automated matching, ownership claims, notifications, and return process tracking.

For the frontend, three widely used technologies were considered: React, Vue.js, and Angular. For backend development, Node.js with Express, Django, and Spring Boot were compared.

The technologies were evaluated according to development complexity, ecosystem, maintainability, suitability for REST API integration, and their applicability to the requirements of the proposed system.

## 5.2. Frontend Technology Comparison

The frontend of the proposed system will provide interfaces for several user roles and workflows. Users will need to create and manage lost item reports, review potential matches, submit ownership claims, receive notifications, and track report and claim statuses. Organization employees and administrators will require separate interfaces for managing found items, reviewing claims, and monitoring organizational activities.

React, Vue.js, and Angular were considered as possible frontend technologies.

| Criterion | React | Vue.js | Angular |
| --- | --- | --- | --- |
| Development Complexity | Medium | Low | High |
| Learning Curve | Medium | Low | High |
| Ecosystem | Very Large | Large | Large |
| Component-Based Development | Yes | Yes | Yes |
| Dynamic Interface Development | High | High | High |
| Maintainability | High | High | High |
| Suitability for the Proposed System | High | High | High |

React is a JavaScript library for developing component-based user interfaces. Its component model allows interfaces to be divided into reusable elements, which is useful for implementing forms, item cards, dashboards, status indicators, notifications, and administrative interfaces.

Vue.js also provides a component-based development model and has a relatively accessible learning curve. It is suitable for developing interactive web applications and could satisfy the frontend requirements of the proposed system.

Angular provides a more comprehensive framework with built-in functionality for developing large web applications. However, its additional architectural complexity may introduce unnecessary development overhead for the current project scope.

Based on these considerations, React was selected as the frontend technology. Its component-based architecture, ecosystem, and suitability for dynamic interfaces make it appropriate for the planned user and organization workflows.

## 5.3. Backend Technology Comparison

The backend of the proposed system will be responsible for processing application requests and implementing the main business logic.

Its responsibilities will include user authentication, authorization, organization management, lost and found item processing, automated identification of potential matches, ownership claim management, notification processing, and return status tracking.

Three backend alternatives were considered: Node.js with Express, Django, and Spring Boot.

| Criterion | Node.js + Express | Django | Spring Boot |
| --- | --- | --- | --- |
| Primary Language | JavaScript | Python | Java |
| Development Complexity | Low to Medium | Medium | High |
| REST API Development | High | High | High |
| Authentication and Authorization Support | High | High | High |
| Ecosystem | Very Large | Large | Very Large |
| Integration with React | High | High | High |
| Flexibility | High | High | High |
| Suitability for the Proposed System | High | High | High |

Node.js provides a JavaScript runtime environment for server-side application development, while Express provides a lightweight framework for organizing routes, middleware, and API functionality.

Django is a Python-based web framework that provides many built-in capabilities, including authentication and administrative functionality. It is suitable for structured web application development but would introduce an additional programming language into the selected technology stack.

Spring Boot is a Java-based framework commonly used for developing structured and scalable backend applications. It provides extensive functionality for API development and application security. However, its configuration and architectural complexity may be greater than necessary for the current project scope.

Based on the comparison, Node.js with Express was selected for backend development. It provides sufficient flexibility for implementing REST APIs and the business logic required by the proposed system while allowing JavaScript to be used across both the frontend and backend.

## 5.4. Selected Technology Stack

Based on the conducted comparison, React and Node.js with Express were selected as the main technologies for implementation of the proposed system.

| System Layer | Selected Technology | Main Purpose |
| --- | --- | --- |
| Frontend | React | Development of interactive user, employee, and administrator interfaces |
| Backend | Node.js + Express | REST API development and implementation of server-side business logic |

React will be responsible for the client-side interface and interaction with users. The frontend will communicate with the backend through REST API requests.

Node.js with Express will process these requests and implement the main application logic, including authentication, authorization, item management, matching operations, ownership claims, and return process tracking.

Using JavaScript across both layers also provides a consistent development environment and reduces the need to maintain different programming languages for the client and server components.

## 5.5. Justification for the Proposed System

The selected technology stack is suitable for the architecture and functionality defined in the Project Proposal.

The proposed platform contains several interactive workflows rather than only static pages. React supports the development of reusable interface components for lost and found reports, item search results, potential match lists, ownership claim forms, status tracking, notifications, and organization dashboards.

Node.js with Express provides the server-side flexibility required to implement the system's main workflows. REST API endpoints can be organized around major system entities and operations, including users, organizations, lost items, found items, potential matches, claims, and return processes.

The selected stack is also appropriate for implementing role-based access restrictions. The backend can determine whether a request is performed by a general user, organization employee, organization administrator, or platform administrator before allowing access to protected operations and information.

The automated matching mechanism planned for the initial implementation does not require a separate machine learning infrastructure. As defined in the Project Proposal, the initial approach can use structured item attributes and similarity or rule-based scoring. This logic can be implemented within the backend and extended later if evaluation demonstrates a need for more advanced matching techniques.

The technology selection therefore reflects the current functional scope of the project rather than assuming requirements for large-scale or computationally complex infrastructure that have not yet been established.

## 5.6. Conclusion

This section compared three frontend technologies and three backend technologies for the proposed Multi-Organization Lost and Found Management System.

React, Vue.js, and Angular were considered for frontend development, while Node.js with Express, Django, and Spring Boot were considered for backend development.

React was selected for the frontend because of its component-based development model, ecosystem, maintainability, and suitability for interactive web interfaces. Node.js with Express was selected for the backend because it supports flexible REST API development and allows the project to use JavaScript across both client-side and server-side development.

The selected React and Node.js with Express stack provides an appropriate technical foundation for implementing the current requirements of the proposed system. Additional technology decisions, including database and deployment technologies, will be defined according to the system architecture and implementation requirements.
