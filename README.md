# CS-255 System Analysis and Design | SNHU Portfolio

## DriverPass — System Analysis & Design Portfolio

### Project Summary

DriverPass was the client for this project — a company that wanted to provide comprehensive driver training to help students pass their driving tests at the DMV. They identified a gap in the market: over 65% of students fail their driving tests because they only study previous tests without practical preparation. DriverPass wanted a cloud-based system that would offer online practice exams, online class content, and on-the-road driving lessons, all managed through a single web portal.

The system I designed needed to handle customer registration, appointment scheduling, payment processing, practice test administration, reporting, and DMV integration. It required role-based access for four user types: the owner (Liam), the IT admin (Ian), the secretary, and customers. The system also needed to support three training packages, track driver/car assignments, maintain a full audit trail of all reservation changes, and automatically receive DMV content updates.

### What I Did Particularly Well

I think the strongest part of my work was the requirements gathering phase. The business requirements document thoroughly captured the client's needs directly from the interview transcript — every functional and nonfunctional requirement traces back to something the client explicitly asked for. I was careful to distinguish between what the client wanted in the initial build versus future features, which kept the scope realistic. On the system design side, the UML diagrams (use case, activity, sequence, and class) provide a clear and complete picture of how the system should function, and the technical requirements section translates those diagrams into concrete hardware, software, and infrastructure decisions.

### What I Would Revise

If I could revise one part, it would be the nonfunctional requirements section — specifically the performance and scalability requirements. While I specified that the system should load within three seconds and be cloud-hosted, I did not define specific concurrent-user targets or peak-load scenarios. DriverPass would likely see traffic spikes during peak DMV test preparation seasons, and the design should have included more specific scalability requirements (e.g., supporting X concurrent users during peak hours with auto-scaling). I would also refine the DMV integration requirements to specify the exact API protocol and data format, since the current design assumes the DMV provides a notification mechanism without defining how that mechanism works.

### Interpreting the User's Needs

I interpreted the user's needs by carefully analyzing the interview transcript and identifying every explicit request, constraint, and preference the client mentioned. Each requirement in the business requirements document maps directly to a statement from the client. I then translated those requirements into system design components — use cases for each user role, activity diagrams for key workflows, a class diagram for the data model, and technical requirements for the infrastructure. The role-based access control system, the audit trail, the package management feature, and the DMV integration all came directly from what the client described.

Considering the user's needs is critical because a system that does not meet the user's actual requirements is a failure regardless of how technically elegant it is. In this project, the client had very specific operational needs — four distinct user roles, three training packages, DMV content synchronization, audit trails for accountability. If any of those were missed or misunderstood, the system would not function for the business. Designing without understanding the user leads to wasted development time, unusable features, and systems that solve the wrong problem.

### Approach to Software Design

My approach to designing software starts with thorough requirements gathering — understanding who the users are, what they need the system to do, and what constraints exist. I then translate those requirements into visual models (UML diagrams) before writing any code or specifying any infrastructure. This helps catch design flaws early, when they are cheap to fix. I break the system into functional components and think about how they interact.

In the future, I would incorporate more iterative validation — sharing early design drafts with the client or stakeholders to confirm the interpretation is correct before investing in detailed design. I would also use prototyping tools to create wireframes alongside the UML diagrams, giving the client a visual sense of the interface before development begins. Finally, I would apply risk assessment earlier in the process, identifying integration risks (like the DMV API dependency) and defining fallback strategies before they become blockers during implementation.

---

## Repository Contents

- `DriverPass Business Requirements Document.docx` — Project One: business requirements gathered from the DriverPass client interview
- `CS255_ProjectTwo_SystemDesignDocument.docx` — Project Two: system design document with UML diagrams and technical requirements

## AI Usage Disclosure

Generative AI tools were used to support the drafting and refinement of these project documents. AI assistance was used for initial research, structuring content, and reviewing clarity. All content was reviewed and finalized by the author.
