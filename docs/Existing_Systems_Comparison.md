# Existing Systems Comparison

**Project Title:** Design and Development of a Web-Based Multi-Organization Lost and Found Management System with Automated Item Matching, Ownership Verification, and Return Process Tracking

**University:** Astana IT University  
**Program:** Software Engineering  
**Team Members:** Makhanbetiyar Begina Berikbolkyzy (SE-2427); Amralina Kamila (SE-2427)  
**Supervisor:** Alua Bauyrzhanovna Myrzakerimova  
**Date:** October 2026

## 1. Introduction

Lost and found management is an important administrative process for universities, shopping malls, transport operators, hotels, and other public organizations. Traditional approaches often depend on manual records, telephone inquiries, emails, and separate organizational procedures. Digital platforms can improve this process by centralizing information, supporting item identification, and facilitating communication between individuals and organizations.

Several commercial lost and found management systems already provide online reporting, automated item matching, ownership verification, and return management. Examining these systems is necessary to understand existing solutions and identify suitable approaches for the proposed diploma project.

This analysis compares four existing platforms: iLost, NotLost, Troov, and ReclaimHub. The platforms were selected because they provide relevant lost and found management functionality and have publicly accessible official documentation.

The comparison uses nine consistent criteria derived from the proposed system's intended functionality. It evaluates documented capabilities and identifies areas that require further consideration during system design.

The analysis is based on publicly available official product information reviewed in October 2026. Where a capability could not be established from the reviewed documentation, it is marked as Not Verified rather than assumed to be unavailable.

## 2. Overview of Existing Systems

2.1. iLost

**Official website:** https://ilost.co/

iLost is an online lost and found platform connecting individuals who have lost belongings with organizations and individuals who have registered found items. It is used by participating organizations across different sectors, including transportation, public services, and entertainment venues [1].

A major feature of iLost is its public search interface. Users can search registered found items, including records associated with different participating organizations. Organizations and individual finders can register found belongings with descriptions and other identifying information.

When users identify an item that may belong to them, they can submit an ownership claim. The claimant is encouraged to provide details that are not immediately visible in the item's public description. The person or organization holding the item reviews this information and decides whether to approve the claim [2].

After ownership confirmation, the system can support collection arrangements or shipment, depending on the options provided by the organization [3].

The standard iLost workflow emphasizes searching registered found items. However, its documentation also describes organization-dependent loss reporting and an iLost Alert mechanism. Therefore, lost item reporting is treated as partially supported rather than universally available through the same workflow [4].

For the proposed project, iLost is especially relevant because it demonstrates how found item records from multiple participating organizations can be made accessible through a shared search platform.

### 2.2. NotLost

**Official website:** https://notlost.com/

NotLost is a cloud-based lost property management platform designed for businesses and organizations. It supports digital registration, management, matching, and return of lost belongings [5].

The platform provides online lost item reporting forms, allowing customers to submit information about missing belongings. Organizational staff can register found items using image recognition technology, which assists with item identification and documentation.

One of its key features is an automated matching engine that compares lost item inquiries with registered found items and suggests potential matches. This reduces the need for staff to compare every report manually [5].

NotLost also provides automated email notifications, configurable item fields, digital item history, management reports, and return arrangements. Organizations can manage information across multiple sites and service points, while user roles allow access to be controlled according to staff responsibilities [6].

According to the official FAQ, customers cannot publicly browse the organization's found item inventory; only designated staff members can view and modify those records. The platform also currently supports English only. Final ownership validation remains the responsibility of the organization using the software [7].

NotLost is a useful reference for automated matching, administrative dashboards, role-based access, and return process management.

### 2.3. Troov

**Official website:** https://troov.com/en/

Troov is a lost and found platform that connects people who have lost belongings with participating organizations and locations. It provides digital reporting and matching services designed to facilitate item recovery [8].

Users can submit lost item reports containing information such as item category, location, description, and photographs. Organizations can register found items, and the platform uses an automated matching algorithm to identify potential relationships between lost and found reports.

When a potential match is identified, the user may be required to answer an ownership verification question. The participating organization reviews the information before authorizing the return of the item [9].

Troov also supports collection and, where offered by the participating organization, delivery arrangements. Its professional tools include item history, document management, team management, and QR-code-based storage support [10].

An important characteristic of Troov is that its matching process distinguishes potential matches from validated matches. The platform does not treat an automated suggestion as sufficient proof of ownership.

For the proposed project, Troov provides a particularly relevant example of combining automated item matching with a structured ownership verification process.

### 2.4. ReclaimHub

**Official website:** https://reclaimhub.com/

ReclaimHub is a cloud-based lost property management platform designed for businesses and organizations. It provides tools for recording, managing, and returning lost and found belongings [11].

Organizations can register found items and manually add reports of missing belongings. ReclaimHub also provides an embeddable reporting widget that allows customers to submit lost item reports through an organization's website [12].

The platform includes an automated matching mechanism that suggests potential matches between lost and found records. Staff can review suggested matches and confirm them before notifying the potential owner.

Additional features include item photographs, configurable categories, notifications, reporting tools, and processes for handling items that remain unclaimed after a specified period [11].

ReclaimHub supports organizational lost property operations, but the reviewed public documentation does not establish that it provides a unified public search environment across multiple independent organizations.

The platform is relevant to the proposed project because it demonstrates a relatively straightforward workflow for registering reports, identifying potential matches, and managing item returns.

## 3. Comparison Criteria

The selected systems were evaluated using nine criteria related to the proposed project's functional requirements.

## 1. Lost Item Reporting: The ability to submit a digital report describing a missing item.

## 2. Found Item Registration: The ability to register found belongings with relevant details.

## 3. Multi-Organization Public Search: The ability for users to search item records from multiple independent organizations through a shared public interface.

## 4. Automated Item Matching: The ability to automatically identify or suggest potential matches between reports.

## 5. Ownership Verification: The presence of a process for reviewing ownership claims before item release.

## 6. Return Process Management: Support for organizing collection, delivery, or other return activities.

## 7. Role-Based Access Control: Documented support for different staff permissions or access roles.

- **Automated Notifications:** Automatic communication about item reports, matches, claims, or recovery.

- **Public Found Item Search:** The ability for ordinary users to browse or search registered found items without staff assistance.

**The following classification was applied:**

- Yes: The capability is explicitly supported by the reviewed official documentation.

- Partial: The capability is available with documented restrictions or only for particular workflows.

- Not Verified: The reviewed official documentation does not provide sufficient evidence to confirm the capability.

A Not Verified classification does not establish that the feature is absent.

## 4. Comparative Analysis

**Table 1. Feature Comparison of Existing Lost and Found Platforms**

| Comparison Criterion | iLost | NotLost | Troov | ReclaimHub |
|---|---|---|---|---|
| Lost Item Reporting | Partial | Yes | Yes | Yes |
| Found Item Registration | Yes | Yes | Yes | Yes |
| Multi-Organization Public Search | Yes | Not Verified | Not Verified | Not Verified |
| Automated Item Matching | Not Verified | Yes | Yes | Yes |
| Ownership Verification | Yes | Yes | Yes | Not Verified |
| Return Process Management | Yes | Yes | Yes | Yes |
| Role-Based Access Control | Not Verified | Yes | Not Verified | Not Verified |
| Automated Notifications | Yes | Yes | Yes | Yes |
| Public Found Item Search | Yes | No | Not Verified | Not Verified |

**Table notes:**

For iLost, the standard workflow focuses on public search and ownership claims, although additional loss-reporting options are documented. The reviewed sources do not establish an automated lost–found matching mechanism equivalent to those explicitly advertised by NotLost, Troov, and ReclaimHub.

For NotLost, support for multiple sites and organizational customers is documented, but this does not necessarily mean users can search found items across independent organizations through one public interface. Its official FAQ explicitly states that found item inventories are visible only to designated staff.

For Troov, the availability of multiple partner organizations is documented, but the reviewed sources do not establish a unified public catalogue of their found item records. Team management is advertised, but the exact role-permission structure is not described sufficiently to confirm granular role-based access control.

For ReclaimHub, organizational item management and automatic matching are documented. However, the reviewed sources do not establish the details of ownership verification, granular staff permissions, or public cross-organization search.

## 5. Strengths and Limitations of Existing Systems

5.1. iLost

The main strength of iLost is its shared public search environment. Users can search registered found belongings associated with participating organizations, submit claims, and communicate with the responsible finder.

The platform also supports a structured verification process in which the organization or individual holding the item makes the final ownership decision.

However, the standard lost item reporting workflow is more restricted than the found item search workflow. In addition, the reviewed sources do not confirm the use of an automated matching engine comparable to the systems explicitly described by other providers.

These observations suggest that the proposed project should consider how to support both lost and found reporting within a consistent interface while maintaining clear ownership verification procedures.

### 5.2. NotLost

NotLost provides a comprehensive set of organizational management functions. Its strengths include automated matching, image recognition, online reporting, user roles, digital history, notifications, and return management.

The platform is particularly suitable for organizations that need to process large volumes of lost property reports.

However, NotLost does not provide public access to the organization's found item inventory. Its documentation also states that the software currently supports English only.

These characteristics are relevant to the proposed project when considering whether users should be able to search found items independently and whether additional interface languages should be supported.

### 5.3. Troov

Troov combines digital reporting, automated matching, and structured ownership verification. Its verification process distinguishes potential matches from confirmed ownership claims.

The platform also supports recovery arrangements and administrative tools for participating organizations.

However, the reviewed documentation does not provide sufficient information about a shared public found item catalogue or the exact structure of staff access permissions.

The proposed project can use Troov's approach as a reference for separating automated matching from final ownership verification.

### 5.4. ReclaimHub

ReclaimHub provides a clear organizational workflow for registering lost and found items, identifying possible matches, sending notifications, and managing returns.

Its embeddable reporting widget is particularly useful for organizations that want customers to submit reports through an existing website.

However, the reviewed public documentation does not establish whether ReclaimHub supports a unified public search interface across independent organizations or a detailed ownership verification workflow.

The platform therefore provides a useful reference for practical item management and automated matching, while some capabilities require further investigation.

## 6. Justification of the Proposed System

The comparison demonstrates that existing commercial platforms already provide many of the functions planned for the proposed diploma project. Automated matching, online reporting, ownership verification, notifications, and return management are established approaches.

Therefore, the proposed system should not be presented as the first platform to combine these concepts.

Instead, the project aims to design and implement a web-based multi-organization lost and found management system based on a clearly defined set of user and organizational requirements.

The intended design includes a unified interface for submitting lost and found reports, searching relevant item records, identifying potential matches, and tracking ownership claims.

A central architectural requirement is the separation of organizational data and administrative responsibilities. Each participating organization should be able to manage its own item records and verification decisions, while the platform should provide appropriate shared search functionality.

The automated matching mechanism will identify possible matches using selected item attributes. A suggested match will not be treated as proof of ownership. Instead, the system will support a separate verification procedure before an item is returned.

The project will also define item and claim statuses to make the recovery process more transparent. These statuses may include Reported, Potential Match, Claim Submitted, Under Verification, Approved, Rejected, and Returned.

The project's contribution will be demonstrated through its implemented functionality, architectural decisions, access control mechanisms, and evaluation results. Its effectiveness will be assessed against the requirements and testing criteria established during the development process.

If multilingual support is included in the final requirements, it may also improve accessibility for users in Kazakhstan. However, such support should be treated as a planned feature rather than an implemented capability until development and testing are completed.

## 7. Conclusion

This analysis compared four existing lost and found management platforms: iLost, NotLost, Troov, and ReclaimHub.

iLost demonstrates the value of public search across participating organizations and structured ownership claims. NotLost provides extensive automation, image recognition, role-based access, and organizational management features. Troov combines automated matching with ownership verification questions and recovery workflows. ReclaimHub offers practical tools for registering reports, suggesting matches, notifying users, and managing returns.

The comparison shows that the proposed diploma project builds upon established approaches rather than introducing entirely new lost and found management concepts.

The proposed system will focus on integrating selected capabilities into a coherent multi-organization web platform with defined organizational permissions, automated matching, ownership verification, and return process tracking.

The final value of the project will depend on how effectively these capabilities are implemented, tested, and aligned with the needs of its intended users.

## References

[1] iLost, “I Have Lost Something, What Can I Do?” iLost Help Center, 2026. https://support.ilost.co/en/articles/341042-i-have-lost-something-what-can-i-do

[2] iLost, “How Do I Submit a Claim for a Found Item?” iLost Help Center, 2026. https://support.ilost.co/en/articles/365835-how-do-i-submit-a-claim-for-a-found-item

[3] iLost, “What Is the Process for Retrieving My Found Property?” iLost Help Center, 2026. https://support.ilost.co/en/articles/341052-what-is-the-process-for-retrieving-my-found-property

[4] iLost, “How to Share a Lost Item Message?” iLost Help Center, 2026. https://support.ilost.co/en/articles/341038-how-to-share-a-lost-item-message

[5] NotLost, “NotLost: Lost Property Management Software.” https://notlost.com/

[6] NotLost, “Lost and Found Software Features.” https://notlost.com/lost-and-found-software-features/

[7] NotLost, “Frequently Asked Questions.” https://notlost.com/faq-lost-property-software-and-saas-lost-and-found-solution/

[8] Troov, “Lost Property: Find Your Property on Troov.” https://troov.com/en/

[9] Troov, “What Is a Match?” Troov Help Center. https://troov.com/en/faq/take-it-easy/what-is-a-match

[10] Troov, “Lost Property Management Software.” https://troov.com/en/lost-properties-manager

[11] ReclaimHub, “Lost Property Management Software.” https://reclaimhub.com/

[12] ReclaimHub, “How It Works.” https://reclaimhub.com/how-it-works/
