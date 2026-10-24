# 9. Verification and Evaluation Plan

## 9.1. Introduction

This section defines the verification and evaluation plan for the Multi-Organization Lost and Found Management System. The purpose of the plan is to establish how the system will be assessed against the functional and non-functional requirements defined earlier in the project.

At the current stage, this section represents a planned verification approach rather than completed testing. The described procedures will be applied progressively as the system is implemented.

The evaluation focuses on the core functions of the proposed system, including lost and found item management, automated item matching, ownership verification, return process tracking, organization management, notifications, security, usability, and performance.

## 9.2. Verification Objectives

The main objectives of system verification are to:

- verify that implemented functionality corresponds to the defined functional requirements;
- verify that users can create and manage lost item reports;
- verify that found items can be registered and managed by authorized organization representatives;
- evaluate whether the automated matching mechanism produces relevant potential matches;
- verify that ownership claims are processed separately from automated matching;
- verify that private ownership verification information is protected from unauthorized users;
- verify that item return processes can be tracked from claim submission to final return;
- verify role-based access control and organization-level data separation;
- evaluate the usability of the main user workflows;
- evaluate basic system performance and reliability;
- identify defects and inconsistencies before final deployment.

## 9.3. Verification Methods

Several complementary verification methods are planned for the system.

**Functional testing** will verify individual system functions against the functional requirements.

**Integration testing** will verify interactions between the frontend, backend services, data storage, matching functionality, ownership claims, notifications, and return tracking components.

**Role-based access testing** will verify that functionality and data are available only to authorized user roles.

**Scenario-based testing** will evaluate complete workflows such as reporting a lost item, identifying a potential match, submitting an ownership claim, and completing the return process.

**Usability evaluation** will assess whether the main interfaces and workflows can be understood and completed by intended users.

**Performance testing** will be used to evaluate basic response times and the behavior of search and matching operations under representative prototype workloads.

## 9.4. Functional Testing Plan

Functional testing will be based directly on the requirements defined in the Requirements Specification.

| Test ID | Function | Related Requirements | Expected Result |
|---|---|---|---|
| FT-01 | User registration and login | FR-01–FR-05 | User can authenticate and access functionality appropriate to the assigned role. |
| FT-02 | Lost item report creation | FR-06–FR-08 | User can create a lost item report containing the required item information. |
| FT-03 | Found item registration | FR-09–FR-12 | Authorized employee can register and update a found item record. |
| FT-04 | Search and filtering | FR-13–FR-16 | User can search and filter appropriate item records without accessing restricted information. |
| FT-05 | Automated matching | FR-17–FR-21 | System identifies and presents potential matches using defined matching rules or similarity scoring. |
| FT-06 | Ownership claim submission | FR-22–FR-28 | User can submit ownership evidence and an authorized employee can review the claim. |
| FT-07 | Return process tracking | FR-29–FR-32 | Approved item return can be tracked through the defined return statuses. |
| FT-08 | Notifications | FR-33–FR-36 | Relevant users receive notifications for significant status changes. |
| FT-09 | Organization management | FR-37–FR-43 | Organization and platform administration functions respect role and organization boundaries. |

Each test case will include input data, execution steps, expected results, actual results, and pass/fail status when testing is performed.

## 9.5. Automated Matching Evaluation

The automated matching mechanism is one of the central functions of the proposed system. The initial implementation is expected to use rule-based comparison and similarity scoring rather than requiring a machine learning model.

The evaluation will use prepared pairs of lost and found item records. These records will contain characteristics such as:

- category;
- brand;
- model;
- color;
- location;
- lost or found date;
- descriptive characteristics.

The evaluation will determine whether records that describe the same or sufficiently similar item receive higher matching scores than unrelated records.

The following scenarios will be considered:

1. records with almost identical characteristics;
2. records with several matching characteristics and several missing attributes;
3. records with similar categories but different identifying characteristics;
4. records from relevant nearby locations and dates;
5. clearly unrelated records.

The evaluation will examine the ordering and relevance of suggested matches. The purpose is not to establish ownership automatically, but to determine whether the mechanism can effectively narrow the set of possible found items that should be reviewed by the user.

## 9.6. Ownership Verification Evaluation

Ownership verification will be evaluated independently from automated item matching.

This distinction is important because a high similarity score indicates only that two records may refer to the same item. It does not prove that the person submitting a claim is the legitimate owner.

Testing will verify that:

- a user can submit an ownership claim for a potential match;
- additional verification information can be provided with the claim;
- private identifying characteristics are not exposed through public search;
- authorized organization employees can review submitted verification information;
- unauthorized users cannot access private ownership evidence;
- an employee can approve or reject a claim;
- claim status is visible to the appropriate user;
- approval of ownership is not performed automatically solely on the basis of a matching score.

Test scenarios will include valid claims, incomplete claims, claims containing incorrect identifying information, and unauthorized attempts to access verification data.

## 9.7. Usability Evaluation

Usability evaluation will focus on the main workflows represented in the initial user interface prototype.

The planned evaluation will consider whether users can understand and complete tasks such as:

- navigating the User Dashboard;
- creating a lost item report;
- searching for found items;
- reviewing potential matches;
- submitting an ownership claim;
- checking claim and return status.

Evaluation criteria will include clarity of navigation, clarity of labels and status information, number of unnecessary steps, consistency between screens, and user understanding of the difference between a potential match and verified ownership.

Feedback obtained during future usability evaluation may be used to refine the Figma prototype and implemented user interface.

## 9.8. Security and Access Control Verification

Security verification will focus on the security and privacy requirements defined in the Requirements Specification.

The planned tests will verify that:

- unauthenticated users cannot access protected functionality;
- role-restricted operations cannot be performed by unauthorized users;
- organization employees can access only operations permitted for their organization;
- organization administrators cannot administer unrelated organizations;
- private ownership verification information is not publicly accessible;
- user input is validated before processing;
- passwords are not stored as plain text;
- attempts to access protected resources without appropriate authorization are rejected.

Particular attention will be given to organization-level isolation because the system is designed to support multiple independent participating organizations.

## 9.9. Performance Evaluation

Basic performance evaluation will be conducted after the main system functionality has been implemented.

The evaluation will focus on operations that are expected to be frequently used or computationally significant, including:

- loading the user dashboard;
- searching and filtering item records;
- submitting lost and found item reports;
- calculating potential item matches;
- retrieving claim and return status information.

Response times will be measured under representative prototype conditions. The purpose of this evaluation will be to identify operations that cause noticeable delays and require optimization rather than to claim production-scale performance at the prototype stage.

## 9.10. Requirements Traceability

Verification activities will be connected to the requirements defined in Chapter 6.

Functional requirements FR-01–FR-43 will primarily be evaluated through functional, integration, and scenario-based testing.

Non-functional requirements NFR-01–NFR-20 will be evaluated through security checks, usability evaluation, performance measurements, architecture review, maintainability assessment, and interface compatibility checks where applicable.

Maintaining this traceability will make it possible to identify which requirements have been verified and which require additional evaluation during later development stages.

## 9.11. Acceptance Criteria

The prototype will be considered ready for the next project stage when the implemented core functionality satisfies the following general acceptance criteria:

- core user workflows can be completed without critical functional errors;
- authentication and role-based access restrictions operate as intended;
- lost and found item records can be created and retrieved correctly;
- search and filtering return relevant records;
- the matching mechanism produces reasonable candidate matches for representative test cases;
- matching results do not automatically establish ownership;
- private verification information remains restricted to authorized workflows;
- ownership claims can be reviewed and assigned an appropriate status;
- return process statuses can be recorded and tracked;
- organization-level access restrictions prevent unauthorized cross-organization administration;
- the primary interfaces remain usable on supported modern web browsers;
- no unresolved critical defects prevent completion of the primary system workflows.

More specific quantitative thresholds may be established after the prototype implementation and representative test data are available.

## 9.12. Conclusion

The proposed verification and evaluation plan provides a structured approach for assessing the Multi-Organization Lost and Found Management System against its functional and non-functional requirements.

The plan combines functional testing, integration testing, access-control verification, scenario-based evaluation, matching evaluation, usability assessment, and performance testing. Particular attention is given to automated matching, ownership verification, and multi-organization access control because these functions distinguish the proposed system from a basic lost and found listing platform.

The verification activities described in this section will be performed progressively during implementation. Their results will later provide evidence for evaluating the correctness, usability, security, and overall effectiveness of the developed system.
