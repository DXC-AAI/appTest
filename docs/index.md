# **appTest**

## Project Description

This is an application with a pair of servers one webserver and one application server

- [**appTest**](#cookiecutterproject_name)
  - [Project Description](#project-description)
  - [How to use the runbook](#how-to-use-the-runbook)
  - [Introduction](#introduction)
    - [Introduction/Overview](#introductionoverview)
    - [Data Flow Diagram](#data-flow-diagram)
    - [Data Flow Diagram](#data-flow-diagram-1)
  - [Apendix C. Document Revision Information](#apendix-c-document-revision-information)
  - [Apendix D. Document Ownership Matrix](#apendix-d-document-ownership-matrix)
  - [Apendix E. Disclaimer](#apendix-e-disclaimer)

## How to use the runbook

- On the left you have the different sections of the documents
- On the right you have the table of contents of each section

|     |                   | |                  |     |
|-----|-------------------|-|------------------|-----|
| <-- | Document Sections | |                  |     |
|     |                   | |Table of contents | --> |

## Introduction

**This section is to be completed to provide a brief overview of the application product being deployed.**

This Run Book is based on Architecture Document **\[**filename**\]** Version **\[**n.n**\]**.

### Introduction/Overview

| Phase 1 - Infrastructure/OS | Phase 2 – Application Phase / Non Production | Phase 3 – Production |            |          |             |            |          |             |
| --------------------------- | -------------------------------------------- | -------------------- | ---------- | -------- | ----------- | ---------- | -------- | ----------- |
| Virtual                     | Server                                       | Blade                | Middleware | Database | Application | Middleware | Database | Application |
| R                           | R                                            | R                    | U          | U        | U           |            |          |             |

***\[**The Run Book is a document that is used to implement new servers and support an application after it is in steady state in a hosting environment. It is very important that accurate and thorough information is supplied when building the Run Book. The technical members of the project team involved in the deployment and steady state management of the application should complete this document. It is also important to note that a specific application may reference other Run Books, especially if that application makes use of shared infrastructure or shared applications. In other words, a Run Book can reference another Run Book.*

*Finally, it is the responsibility of all parties involved in the implementation and support of an application to maintain current and accurate information, versioning the Run Book as appropriate.*

*Help with this document can be obtained from the AA Project Manager and/or AA Application Owner, or Technologist who is assigned to the project. In this section provide an overview of the functionality provided by the application.**\]***

### Data Flow Diagram

| Phase 1 - Infrastructure/OS | Phase 2 – Application Phase / Non Production | Phase 3 – Production |            |          |             |            |          |             |
| --------------------------- | -------------------------------------------- | -------------------- | ---------- | -------- | ----------- | ---------- | -------- | ----------- |
| Virtual                     | Server                                       | Blade                | Middleware | Database | Application | Middleware | Database | Application |
| IF                          | IF                                           | IF                   | U          | U        | U           |            |          |             |

***\[**In this section, illustrate the high-level operation of the application. From Architecture document**\]***

### Data Flow Diagram

| Phase 1 - Infrastructure/OS | Phase 2 – Application Phase / Non Production | Phase 3 – Production |            |          |             |            |          |             |
| --------------------------- | -------------------------------------------- | -------------------- | ---------- | -------- | ----------- | ---------- | -------- | ----------- |
| Virtual                     | Server                                       | Blade                | Middleware | Database | Application | Middleware | Database | Application |
| IF                          | IF                                           | IF                   | U          | U        | U           |            |          |             |

***\[**Provided by Infrastructure Engineer. Packet flows diagrams will include server and/or VM names and IP addresses. Include any physical/packet flow diagrams that are appropriate**\]***


## Apendix C. Document Revision Information

The information below is to be included with all versions of this document. Remember to update the cover page with each version.

| Prepared By   | Date     | Version |
|---------------|----------|---------|
| Barbara Doyle | 09/01/09 | 3.3     |

| Revised By    | Date     | Revision Reason                                                                                                                                                                                                                                                                                                                                                                                                                                                                                | Version |
|---------------|----------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------|
| Barbara Doyle | 05/01/08 | Added Section 3.12 (Citrix), Moved reference material to appendices and created heading. styles for appendices.                                                                                                                                                                                                                                                                                                                                                                                | 3.3     |
| Barbara Doyle | 07/08/08 | Replaced Section 3.11 (Storage) with updated information to include SAN (3.11.1) and NAS (3.11.2) specific information.                                                                                                                                                                                                                                                                                                                                                                        | 3.4     |
| Barbara Doyle | 07/30/08 | Added Tier and Service Environment Descriptions to A3 – Appendix Material                                                                                                                                                                                                                                                                                                                                                                                                                      | 3.4.1   |
| Barbara Doyle | 09/01/09 | Added Section 3.13, Security to include SiteMinder and LDAP information required for building out stage and production. The Oracle table (3.9) was updated to current default values, Enterprise Notification Desk (2.4) and Change and Problem System Application Request (2.5) moved from section 7 (7.3 and 7.4) to section 2 so all contact information is easily located in one area. Added Jan Denton, Plano SMC, 6901 Windcrest, Plano, TX  75024 Phone 972-604-5794 to Section 8, PDC. | 3.5     |
| Barbara Doyle | 11/10/09 | Replaced Appendix A4 with new phase process, Integrate HP phased build matrix into Run Book. Added Phase tables to each activity. Changed title of section 3.1 to Hardware Information. Added section 3.1.1 (Servers) for consistency.                                                                                                                                                                                                                                                         | 4.0     |
| Ben White     | 02/15/11 | Added verbiage to ensure passwords are no longer documented in the Run Book.                                                                                                                                                                                                                                                                                                                                                                                                                   | 4.1     |
| Ben White     | 05/30/13 | Adding additional information to Server Information sub-section 3.1.1 for Maintenance Windows at HPs request, adding new sub-section 3.1.4 to Infrastructure Environment section 3 to capture Unix VM zone information, additional information to Monitoring Section 4, and updating contact information in Section 8.                                                                                                                                                                         | 4.2     |
| Ben White     | 02/05/14 | Making adjustments to title page, Section 2.3 outage severity impact, Section 2.5 Pre-Application Phase Requirement, Section 3 Maintenance Windows, Section 4.4 URL Monitoring, Section 8 Data Center Shipping Procedures, and DRS Rules for VMs.                                                                                                                                                                                                                                              | 4.3     |
| Ben White     | 03/06/14 | Adding vPostgres Sub-Section into Run Book.                                                                                                                                                                                                                                                                                                                                                                                                                                                    | 4.3.1   |
| Ben White     | 09/30/14 | Updating Contact Section 2.5.2 with System ID and Change ID. Updating Backup Section 3.14, and removing Backup special process Section 7.1 completely. Also moving Section 7.2/7.3 to the back of Section 3                                                                                                                                                                                                                                                                                    | 4.3.2   |
| Anne Miller   | 11/2/16  | Added many updates that included Before you start tips, changed some of the requirements for the phases, renamed the phases to include Phase 1, 2 or 3. Most changes made to clarify the document and give clearer instructions. Worked closely with HPE on these revisions.                                                                                                                                                                                                                   | 4.4     |

## Apendix D. Document Ownership Matrix

**Responsibility for completing the various sections in the Run Book document should be clearly defined as being the responsibility of a single owner for each document section. Several resources may be involved in the completion of single Run Book but each section should beassigned as the responsibility of a single owner to avoid any confusion.**

| Document Section                                  | Roles                                | Owner | Status |
|---------------------------------------------------|--------------------------------------|-------|--------|
| 1 Introduction                                    |                                      |       |        |
| 1.1 Introduction/Overview                         | Architect + Application Team         |       |        |
| 1.2 Data Flow Diagram                             | Architect                            |       |        |
| 1.3 Packet Flow Diagram                           | Architect                            |       |        |
| 2 Contact Information (all sections)              |                                      |       |        |
| 2.1 Build Out Contacts                            | Infra Engineer                       |       |        |
| 2.2 Steady State Contacts                         | Application Team                     |       |        |
| 2.3 Outage and Severity Notification              | Application Team                     |       |        |
| 2.4 Enterprise Notification Desk                  | Application Team                     |       |        |
| 2.5 Change and Problem System Application Request | Application Team                     |       |        |
| 3 Infrastructure Environment                      |                                      |       |        |
| 3.1 Server Information Servers Blades VMs UVS     | Infra Engineer + EVS + UVS           |       |        |
| 3.2 Device Network Information Request            | Infra Engineer                       |       |        |
| 3.3 BigIP Configuration                           | Infra Engineer + Load Balancing Team |       |        |
| 3.4 Firewall Configuration                        | Infra Engineer                       |       |        |
| 3.5 IIS Information                               | Infra Engineer +App                  |       |        |
| 3.6 IHS WebServer Information                     | Application Team                     |       |        |
| 3.7 WebSphere Information                         | Application Team                     |       |        |
| 3.8 WebSphere MQ Information                      | Application Team                     |       |        |
| 3.9 Database Information                          |                                      |       |        |
| 3.9.1 Oracle Database Information                 | Infra Engineer + Application Team    |       |        |
| 3.9.2 SQL Database Information                    | Infra Engineer + Application Team    |       |        |
| 3.9.3 vPostgres Information                       | N/A                                  |       |        |
| 3.10 Storage Configuration Information            |                                      |       |        |
| 3.10.1 SAN Information                            | Infra Engineer + Application Team    |       |        |
| 3.10.2 NAS Information                            | Infra Engineer + Application Team    |       |        |
| 3.11 Citrix Presentation Server Information       | Infra Engineer + Application Team    |       |        |
| 3.12 Security                                     |                                      |       |        |
| 3.12.1 SiteMinder                                 | Application Team                     |       |        |
| 3.12.2 LDAP                                       | Application Team                     |       |        |
| 3.13 Backup/Restore Requirements                  | Application Team                     |       |        |
| 3.14 System Implementation Guide                  | Application Team                     |       |        |
| 3.15 DNS Guidelines                               | Application Team                     |       |        |
| 4 System Monitoring                               | Application Team                     |       |        |
| 4.1 Windows 2000/2003 Monitoring                  | Application Team                     |       |        |
| 4.2 UNIX Monitoring                               | Application Team                     |       |        |
| 4.3 Alert Procedures                              | Application Team                     |       |        |
| 4.4 URL Monitoring                                | Application Team                     |       |        |
| 5 Application Installation Procedures             | Application Team                     |       |        |
| 5.1 Application Information                       | Application Team                     |       |        |
| 5.2 Acceptance Test Scripts                       | Application Team                     |       |        |
| 6 Disaster Recovery (all sections)                | Application Team                     |       |        |
| 7.0 Data Center Requirements                      | Infra Engineer                       |       |        |

## Apendix E. Disclaimer 

Run Book for distributed systems

document version 1.0

Date

Prepared by:

American Airlines, Inc.

Department:

Platform Hosting Services

> American Airlines System Development Life Cycle Standard  
> Run Book Template Version 4.4 (Nov 2016)  
> AA SDLC Style Guide Version W1.6 (September 2006)

Copyright © 2009, American Airlines, Inc. All rights reserved. 
Printed in the U.S.A.

This documentation is the confidential and proprietary intellectual property of American Airlines, Inc. Any unauthorized use, reproduction, preparation of derivative works, performance, or display of this document, or software represented by this document is strictly prohibited.

AACargo, AA.com, AAdvantage, AAdvantage Executive Platinum, AAdvantage Gold, AAdvantage Platinum, AAirpass, Admirals Club, American Airlines, American Eagle and the American Airlines logo design are trademarks and/or service marks of American Airlines, Inc.

SABRE is a trademark owned by TSGL Holdings Inc.

All other trademarks, service marks, and trade names are owned by their respective companies
