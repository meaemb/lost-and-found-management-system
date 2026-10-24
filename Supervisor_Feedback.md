# 11. Supervisor Feedback

## 11.1. Overview of Supervisor Feedback

During the initial review of the diploma project, the supervisor provided a generally positive assessment of the selected topic, proposed functionality, and current project documentation. The project was considered appropriate for a Software Engineering diploma because it addresses a practical problem and includes several interconnected technical components.

The initial review also highlighted the importance of further refining selected design decisions and providing more detailed evidence of how the proposed functionality will be implemented and evaluated.

The following subsections summarize the main areas identified by the project team for further clarification and improvement following the general feedback.

## 11.2. Areas for Improvement

### 11.2.1. Database Technology Selection

The current technology comparison provides a justification for selecting React for frontend development and Node.js with Express for backend development. However, the database technology has not yet been selected through a formal comparison.

This decision is important because the system will manage related information about users, organizations, lost and found items, ownership claims, potential matches, and return processes.

**Planned improvement:** The team will compare PostgreSQL, MySQL, and MongoDB based on data relationships, consistency, development complexity, and suitability for the proposed system. The selected database will be justified and reflected in the architecture documentation.

### 11.2.2. Expansion of the User Interface Prototype

The initial Figma prototype presents the User Dashboard, Lost Item Reporting interface, and Found Item Search interface. These screens demonstrate the main structure of the user-facing application.

However, the prototype does not yet fully illustrate the ownership verification process, return tracking, and organization-specific administrative workflows.

**Planned improvement:** The team will extend the prototype to include ownership claim submission, claim review, return status tracking, and an Organization Dashboard. The additional screens will help demonstrate complete interactions between general users and authorized organization employees.

### 11.2.3. More Specific Evaluation Criteria

The existing verification and evaluation plan describes functional testing, automated matching evaluation, security checks, and usability assessment.

However, some acceptance criteria remain qualitative, and quantitative evaluation thresholds have not yet been finalized.

**Planned improvement:** The team will define measurable evaluation criteria for the matching mechanism, including precision and recall on a labeled test dataset. The evaluation plan will also specify representative usability tasks, test scenarios, and criteria for successful completion of core workflows.

### 11.2.4. Clarification of Multi-Organization Access Control

The proposed architecture includes multiple independent organizations within one platform. This creates additional requirements for separating organizational records and controlling employee permissions.

Although the existing requirements describe role-based access control, the exact authorization rules will need to be specified in greater detail during implementation.

**Planned improvement:** The team will prepare a role-permission matrix and define organization-level authorization rules. These rules will be used to verify that employees cannot access restricted administrative information belonging to other organizations.

## 11.3. Feedback Response and Action Plan

The following table summarizes the proposed improvements and their expected outcomes.

| Area | Planned Action | Expected Outcome |
|---|---|---|
| Database selection | Compare PostgreSQL, MySQL, and MongoDB | Justified database choice |
| UX prototype | Add ownership claim, claim review, return tracking, and organization administration screens | More complete demonstration of system workflows |
| Evaluation criteria | Define measurable matching and usability criteria | More objective evaluation plan |
| Access control | Prepare a role-permission matrix and organization-level access rules | Clearer security and authorization design |

These activities will be incorporated into the subsequent development plan and tracked through the project's YouTrack board.

## 11.4. Current Status of Supervisor Review

At the first pre-defense stage, the project documentation has undergone an initial review, and the team has identified areas requiring further clarification and refinement.

The planned improvements do not require changing the overall project topic or its primary objectives. Instead, they focus on strengthening the technical justification, completeness of the prototype, evaluation methodology, and security design.

The team will continue to seek supervisor feedback during subsequent development stages and document additional comments and corresponding revisions as they become available.

## 11.5. Conclusion

The initial review supports continuing development of the proposed Multi-Organization Lost and Found Management System while further refining several technical and methodological decisions.

The identified improvement areas provide a practical basis for the next development stage. Addressing them will strengthen the consistency between the project requirements, system architecture, user interface design, and evaluation plan.
