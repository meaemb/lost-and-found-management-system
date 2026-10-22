# Literature Review

**Project Title:** Design and Development of a Web-Based Multi-Organization Lost and Found Management System with Automated Item Matching, Ownership Verification, and Return Process Tracking

University: Astana IT University

Program: Software Engineering

**Team Members:**

- Makhanbetiyar Begina Berikbolkyzy (SE-2427)
- Amralina Kamila (SE-2427)

Supervisor: Alua Bauyrzhanovna Myrzakerimova

October 2026

## 1. Introduction

 Lost and found management is a common administrative process in universities, shopping malls, transportation facilities, and other public environments. Traditional methods often rely on physical logbooks, informal communication channels, or direct contact with organizational staff. Such approaches may create difficulties in organizing reports, searching for potential matches, and monitoring the status of missing belongings.

Recent studies have investigated digital lost and found management systems, automated record matching, privacy-preserving data processing, and access control mechanisms. These areas are relevant to the development of a platform that allows users to report lost and found items across multiple participating organizations.

This literature review examines 13 publications, including research on existing lost and found applications and technical approaches that may support the proposed system. The analysis focuses on four areas: existing lost and found management solutions, automated item matching, privacy and access control, and the limitations of current approaches.

## 2. Existing Lost and Found Management Systems

 Ballard et al. [1] presented the USTP Panaon Lost and Found Management System, which uses QR codes, a centralized database, and mobile and web functionality to support the recovery of lost belongings in a university environment. The system was evaluated in terms of functionality, reliability, usability, efficiency, and security. The authors reported positive evaluation results while also identifying network dependency and user engagement as challenges. Their study demonstrates the potential benefits of digital item identification and centralized information management. However, the solution focuses on a particular academic institution rather than multiple independent organizations.

Shahzan and Arbaiy [2] developed the UTHM Lost and Found Management System to address the limitations of using informal platforms such as Telegram and WhatsApp for reporting lost belongings. Their work adopts a prototyping approach and describes a web-based solution for managing item reports and administrative activities. The study supports the use of a centralized system for improving the organization of lost and found records. Nevertheless, the proposed application is designed for the operational environment of a single university.

Deepthi et al. [3] described a Smart Lost and Found System for Campus that incorporates fuzzy matching, multiple ownership claims, conversational verification, and administrative escalation. These functions are relevant to the proposed project because identifying a potential match does not automatically establish ownership. A separate claim verification process is necessary before an item can be returned. However, the study is focused on a campus environment, and its applicability to multiple organizations with different administrative procedures requires further investigation.

The Find-It Mall system [4] addresses lost and found management in a retail environment. It combines a public reporting portal, a staff dashboard, and automated email notifications. The application was developed using PHP, MySQL, and Bootstrap, following an Agile development approach. The study demonstrates how digital reporting and communication can support lost and found operations in shopping malls. However, the solution primarily addresses a specific retail environment rather than a shared platform for multiple independent institutions.

These four studies show that digital lost and found systems can improve the organization of reports, communication between users and staff, and administrative management. Their main limitation in relation to the proposed project is their focus on individual campuses or retail environments. Although they provide useful examples of reporting and recovery workflows, they do not establish a fully evaluated approach to coordinating lost and found operations across several independent organizations within one platform.

## 3. Automated Item Matching and Entity Resolution

 Automated matching is an important component of the proposed system because users may describe the same item using different words or incomplete information. For example, one user may report a lost black backpack, while another may register a found dark-colored school bag. A matching mechanism should help identify potentially related reports without treating similarity as proof of ownership.

Papadakis et al. [5] conducted an empirical analysis of eight one-to-one matching algorithms for entity resolution. The study evaluated matching accuracy and computational efficiency using ten real-world datasets and more than 700 similarity graphs. The results demonstrate that the performance of matching algorithms depends on the characteristics of the data and the structure of similarity relationships. This research provides a foundation for understanding how potential lost and found matches could be selected and ranked. However, the algorithms were not specifically evaluated on descriptions of lost belongings. Wu and Li [6] proposed MixER, an entity resolution model that uses latent-space interpolation to generate augmented training examples. The approach aims to improve matching performance when labeled training data is limited or noisy. This is relevant because a newly developed lost and found platform may initially have a relatively small dataset of confirmed matches. Nevertheless, the model requires additional implementation and evaluation before its suitability for this application can be established.

Witschard et al. [7] investigated similarity network analysis for improving the understanding of text similarity calculations. Their study examines how different embedding-based models represent similarities between text documents and introduces a methodology for comparing their results. This research is useful for evaluating alternative approaches to comparing item descriptions. However, its experiments concern general text similarity analysis rather than short and potentially incomplete lost and found reports.

Nananukul et al. [8] examined cost-efficient prompt engineering for unsupervised entity resolution in product matching. Their study evaluated different prompting strategies using large language models and real-world product datasets. The authors found that more detailed and expensive prompts do not necessarily outperform simpler approaches. This finding is relevant when considering whether language-model-based matching would offer sufficient benefits compared with less complex methods. However, the research focuses on product matching and does not directly establish the performance of such techniques in lost and found applications.

Jin et al. [9] proposed an image–text matching approach based on semantic filtering and adaptive adjustment. The method attempts to improve alignment between image regions and textual descriptions and was evaluated using the Flickr30K and MSCOCO datasets. The study is relevant because photographs could provide additional information when searching for lost belongings. Nevertheless, general image–text retrieval datasets differ from photographs of personal belongings, where multiple objects may have nearly identical appearances.

Overall, the reviewed matching research provides several possible approaches, including graph-based matching, learned representations, text embeddings, large language models, and image–text retrieval. However, none of these studies directly establishes which method is most suitable for a multi-organization lost and found platform. The proposed project therefore needs to select and evaluate a matching approach based on its own data, functional requirements, and available development resources.

## 4. Privacy, Data Sharing, and Access Control

 A multi-organization lost and found platform may process personal contact information, item descriptions, photographs, and ownership-related evidence. The system must therefore consider both the protection of user information and the separation of organizational responsibilities.

Khan et al. [10] introduced a privacy-preserved incremental record linkage framework. Their approach combines incremental record linkage with privacy-preserving techniques, including phonetic encoding and generalization. The study addresses the challenge of processing new records while limiting the disclosure of sensitive information. This is relevant because lost and found reports are added continuously, and newly submitted records may need to be compared with existing reports. However, the research does not address the verification of physical item ownership or the management of item returns.

Christen et al. [11] investigated privacy-preserving record linkage using autoencoders. Their approach transforms encoded information to support record comparison while reducing exposure to known attacks against Bloom-filter-based encoding. The study provides a technical perspective on matching records while protecting sensitive data. However, its contribution concerns privacy-preserving record linkage, not ownership verification. Confirming that two records correspond to the same entity is different from confirming that a person owns a particular object.

Zubair et al. [12] proposed an access control mechanism for trusted data sharing in distributed multi-tenant environments. Their approach uses fine-grained policies and dynamic enforcement to control data access between participating entities. Although the research focuses on a distributed data streaming environment associated with 6G systems, its principles are relevant to the proposed platform. A multi-organization lost and found system requires mechanisms that allow authorized staff to manage their organization's records without obtaining unrestricted access to other organizations' information.

Belchior et al. [13] investigated role-based access control for model-driven web applications. Their work integrates RBAC into the Semantic Hypermedia Design Method, providing a foundational example of how authorization requirements can be represented during web application design. Although the publication dates from 2012 and uses an older technical framework, its discussion of role-based permissions remains relevant to distinguishing ordinary users, organizational staff, and system administrators.

These studies demonstrate that privacy and access control are important considerations in systems that process information across multiple entities. However, the reviewed privacy-preserving matching approaches should not be confused with ownership verification. In the proposed project, ownership verification will require a separate process for assessing claims and supporting evidence, while access control will determine which users and staff members may view or manage the relevant information.

## 5. Structured Analysis of Related Publications

 Table 1 summarizes the 13 reviewed publications, their main contributions, limitations in relation to the proposed project, and potential applications.

Table 1. Comparative Analysis of Related Publications

| Ref. | Authors / Year | Research focus | Main contribution | Limitation relative to the proposed project |
|---|---|---|---|---|
| [1] | Ballard et al., 2025 | University lost and found system | QR-based identification, centralized records, mobile/web access | Single-campus scope; network and engagement challenges |
| [2] | Shahzan & Arbaiy, 2025 | Web-based lost and found management | Centralized reporting and administrative functions | Designed for one university |
| [3] | Deepthi et al., 2026 | Smart campus lost and found | Fuzzy matching, claim handling, verification, escalation | Multi-organization applicability not established |
| [4] | Nor Azmi et al., 2025 | Retail lost and found system | Public portal, staff dashboard, email notifications | Focused on a retail environment |
| [5] | Papadakis et al., 2023 | Entity resolution | Comparison of eight one-to-one matching algorithms | Not evaluated on lost and found data |
| [6] | Wu & Li, 2024 | Learning-based entity resolution | Latent-space interpolation and data augmentation | Requires training and domain-specific evaluation |
| [7] | Witschard et al., 2025 | Text similarity | Similarity network analysis and model comparison | Focuses on document similarity rather than item reports |
| [8] | Nananukul et al., 2024 | LLM-based product matching | Evaluation of prompting strategies and costs | Product-domain experiments; model cost considerations |
| [9] | Jin et al., 2024 | Image–text matching | Semantic filtering and adaptive adjustment | Not tested on lost belongings |
| [10] | Khan et al., 2022 | Incremental record linkage | Privacy-preserving linkage of newly added records | Does not address item claims or returns |
| [11] | Christen et al., 2023 | Privacy-preserving record linkage | Autoencoder-based encoding for protected matching | Does not verify physical ownership |
| [12] | Zubair et al., 2024 | Access control and data sharing | Fine-grained access policies for multi-tenant environments | Different technical application domain |
| [13] | Belchior et al., 2012 | Role-based access control | RBAC integration into web application design | Older model-driven Semantic Web framework |

The comparison shows that the reviewed publications address different aspects of the proposed system. Studies [1]–[4] provide practical examples of lost and found workflows, while studies [5]–[9] investigate possible matching approaches. Publications [10]–[13] contribute concepts related to privacy, data sharing, and access control.

The research also highlights an important distinction between identifying a potential match and completing the return process. Matching algorithms can help find similar reports, but additional verification and administrative procedures are necessary before an item is released to a claimant.

## 6. Research Gap

 The reviewed literature demonstrates that web-based lost and found systems can support centralized reporting, administrative management, and item recovery. It also shows that automated record matching and secure data management have been extensively investigated in related technical fields. However, the selected lost and found studies primarily focus on individual universities or retail environments. Meanwhile, the reviewed entity resolution and security publications investigate their respective technical problems independently of lost and found operations.

Within the selected literature, there is limited evidence of an integrated web-based platform that combines all four of the following capabilities:

1. Management of lost and found reports across multiple independent organizations.
2. Automated identification of potential matches between lost and found items.
3. Structured verification of ownership claims before releasing items.
4. Tracking of the return process through clearly defined statuses and administrative actions.

This gap provides the motivation for the proposed project.

The intended contribution is not the development of an entirely new entity resolution algorithm. Instead, the project aims to design and implement a web-based platform that integrates relevant matching, access control, verification, and workflow management concepts into one multi-organization system.

The proposed platform will allow users to submit and search for lost and found reports associated with participating organizations. Authorized organizational staff will manage relevant reports and ownership claims, while system administrators will oversee platform-level operations. Automated matching will help identify possible relationships between reports, and return process tracking will provide visibility into the progress of item recovery.

The effectiveness of these features will need to be assessed through implementation and testing. In particular, the project should evaluate the quality of potential item matches, the correctness of access restrictions, and the completeness of the ownership verification and return workflows.

## 7. Conclusion

 This literature review analyzed 13 publications related to lost and found management, entity resolution, image–text matching, privacy-preserving record linkage, and access control.

Existing lost and found systems demonstrate the benefits of centralized reporting, administrative dashboards, and digital communication. Research on entity resolution provides several approaches for identifying potentially corresponding records, while privacy and access control studies offer principles for managing information securely.

The analysis also identifies limitations in the direct applicability of existing research. Most reviewed lost and found systems are designed for individual organizations, while technical studies on matching and security are not specifically evaluated within lost and found workflows.

These findings support the development of a multi-organization lost and found management platform that combines reporting, automated matching, ownership verification, and return process tracking. The proposed system will adapt and integrate relevant existing approaches, with its effectiveness to be evaluated during the development and testing stages.

## References

[1] J. G. Ballard, J. G. Caw-it, C. S. Daig, K. P. Lasagas, I. J. M. Pabatang, and J. D. Sumaylo, “USTP Panaon Lost and Found Management System,” 2025. https://doi.org/10.5281/zenodo.15045175

[2] N. F. Shahzan and N. Arbaiy, “UTHM Lost and Found Management System,” Applied Information Technology and Computer Science, vol. 6, no. 1, pp. 2307–2319, 2025. https://doi.org/10.30880/aitcs.2025.06.01.129

[3] R. Deepthi, P. Poojitha, J. B. Priyanka, M. O. Prarthana, and B. M. Prithvi, “Smart Lost and Found System for Campus: A Web-Based Approach for Item Recovery and Management,” International Journal of Research in Engineering & Science, vol. 16, no. 1, 2026. https://doi.org/10.5281/zenodo.18246844

[4] S. N. S. B. Nor Azmi, K. Wei Yi, A. S. Kasim, and Z. Ismail, “Find-It Mall: A Web-Based Lost and Found Management System for Malaysian Retail Environments,” International Journal of Research and Innovation in Social Science, vol. 9, no. 12, 2025. https://doi.org/10.47772/IJRISS.2025.91200065

[5] G. Papadakis, V. Efthymiou, E. Thanos, O. Hassanzadeh, and P. Christen, “An Analysis of One-to-One Matching Algorithms for Entity Resolution,” The VLDB Journal, vol. 32, pp. 1369–1400, 2023. https://doi.org/10.1007/s00778-023-00791-3

[6] H. Wu and S. Li, “MixER: Linear Interpolation of Latent Space for Entity Resolution,” Complex & Intelligent Systems, vol. 10, pp. 3–22, 2024. https://doi.org/10.1007/s40747-023-01018-2

[7] D. Witschard, K. Kucher, I. Jusufi, and A. Kerren, “Using Similarity Network Analysis to Improve Text Similarity Calculations,” Applied Network Science, vol. 10, article 8, 2025. https://doi.org/10.1007/s41109-025-00699-7

[8] N. Nananukul, K. Sisaengsuwanchai, and M. Kejriwal, “Cost-efficient Prompt Engineering for Unsupervised Entity Resolution in the Product Matching Domain,” Discover Artificial Intelligence, vol. 4, article 56, 2024. https://doi.org/10.1007/s44163-024-00159-8

[9] R. Jin, T. Hou, T. Jin, J. Yuan, and C. Du, “A Method for Image–Text Matching Based on Semantic Filtering and Adaptive Adjustment,” EURASIP Journal on Image and Video Processing, article 23, 2024. https://doi.org/10.1186/s13640-024-00639-y

[10] S. I. Khan, A. B. A. Khan, and A. S. M. L. Hoque, “Privacy Preserved Incremental Record Linkage,” Journal of Big Data, vol. 9, article 105, 2022. https://doi.org/10.1186/s40537-022-00655-7

[11] V. Christen, T. Häntschel, P. Christen, and E. Rahm, “Privacy-Preserving Record Linkage Using Autoencoders,” International Journal of Data Science and Analytics, vol. 15, pp. 347–357, 2023. https://doi.org/10.1007/s41060-022-00377-2

[12] M. Zubair, M. Sabzevari, V. Khatri, S. Tarkoma, and K. Hätönen, “Access Control for Trusted Data Sharing,” EURASIP Journal on Information Security, article 30, 2024. https://doi.org/10.1186/s13635-024-00178-z

[13] M. Belchior, D. Schwabe, and F. S. Parreiras, “Role-Based Access Control for Model-Driven Web Applications,” Lecture Notes in Computer Science, Springer, 2012. https://doi.org/10.1007/978-3-642-31753-8_8
