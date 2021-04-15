# Appendix A. Reference Material

## A.1 Outage and Severity Definitions

The following table defines priority/severity level definitions for
Century Link Technology Solutions and HP.

| Century Link Technology Solutions Priority/Severity Events                                                                                                                                                                                                                                                                                                                                                                                                           | HPE Severity Codes                                                                                                                                                                                                                                                                                                                                                                                                      |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Priority/Severity 1 Event: An operational request relating to a critical Performance Problem, Network Downtime, or Site Unavailability.                                                                                                                                                                                                                                                                                                                              | Severity 1: An Incident causing a complete interruption or extreme degradation of service delivery with a critical impact to the affected client, environment or business operation. Those affected cannot operate until service delivery is restored.                                                                                                                                                                  |
| Priority/Severity 2 Event: Any event, which has not caused Network Downtime but which may cause Network Downtime if not addressed immediately.  This type of event is generally classified by one or more systems (in a multi system configuration) being down or by American experiencing Performance Problems. This classification of event may occur if the capacity thresholds are exceeded, as mutually identified and defined by Exodus and American Airlines. | Severity 2: An Incident causing a significant interruption or degradation of service delivery, with major impact to the affected client, environment or business operation. There may be an automated or manual contingency plan that allows those affected to achieve partial functionality during the event.                                                                                                          |
| Priority/Severity 3 Event: Any event that has not caused Network downtime or a performance problem, and which event can remain unresolved without causing Network Downtime or a performance problem.  This type of event is generally classified by the failure of a device or sub-system that has had minor impact on site functionality and has not resulted in any performance degradation.                                                                       | Severity 3: An Incident causing a moderate interruption or degradation of service delivery, with moderate impact to the affected client, environment or business operation. While immediate impact is moderate, the risk for increased impact may be apparent. There may be an automated or manual contingency plan that allows those affected to achieve a level approaching normal service delivery during the event. |
| Priority/Severity 4 Event: A routine change request or a request for technical or administrative information.                                                                                                                                                                                                                                                                                                                                                        | Severity 4: An Incident causing a minimal interruption or degradation of service delivery, with minor impact to the affected client, environment or business operation (includes single user issues). An automated or manual contingency plan may be available.                                                                                                                                                         |
|                                                                                                                                                                                                                                                                                                                                                                                                                                                                      | Severity 5: An Incident that does not affect normal service delivery for a client, environment or business operation. No current impact. Includes issues with the potential to cause impact if not proactively addressed, and those that began as a higher severity due to Potential Impact, but were resolved prior to causing Actual Impact.                                                                          |

## A.2 Escalation vs Notification Definitions

Notification is the communication of severity level one or two
system/service problems to those parties needing to know (for FYI, as
opposed to on-call responsibilities to fix a problem; e.g.
Infrastructure Manager is notified of these problems, but does not have
the responsibility to resolve the problem).

Escalation is the communication of any problem with a system or service
to ‘on call’ individuals, who have the responsibility to resolve (fix)
the problem. These individuals are regarded as ‘fix agents’.

## A.3 Tier and Service Environment Descriptions

  - A “Tier 0 Server” or “Co-Location Server” means a Server that is
    operated in a Co-Location Environment. Services for a Tier 0 Server
    are limited to space, power and connectivity, as well as limited
    facilities management, network services, physical access security
    and site support for those services listed in the Tier 0 column
    within this Midrange Service Description. A Tier 0 Server cannot be
    reclassified as Tiers 1 – 5 at any time if a Managed Service
    Provider other than HPE is providing hosting services on the
    specified server.

  - A “Tier 1 Server” or “Development Server” means a Server that is
    operated in a Midrange Development Environment. A Tier 1 Server is
    managed for failures or impending failures. The services provided
    for a Tier 1 Server include all of the services listed in the Tier 1
    column within this Midrange Service Description. The Systems
    Software of a Tier 1 Server will be loaded, however a Tier 1 Server
    will not be managed.

  - A “Tier 2 Server” or “Test Server” means a Server that is operated
    in a Midrange Test Environment. The services provided for a Tier 2
    Server include all of the services listed in the Tier 2 column
    within this Midrange Service Description.

  - A “Tier 3 Server” or “Production-Remote Server” means a Server that
    is operated in a Production Environment, but is not located in an
    HPE managed Data Center. The services provided for a Tier 3 Server
    include all of the services listed in the Tier 3 column within this
    Midrange Service Description. Examples of Tier 3 Servers would
    include Servers located at a remote location such as a reservation
    center or airport.

  - A “Tier 4 Server” or “Production-Standard Server” means a Server
    that is operated in a Production Environment and is located in an
    HPE managed Data Center. The services provided for a Tier 4 Server
    include all of the services listed in the Tier 4 column within this
    Midrange Service Description. Tier 4 Server is the default or
    standard category for a Production Environment Server.

  - A “Tier 5 Server” or “Production-HA Server” means a
    Production-Standard Server with a high availability configuration.
    The services provided for a Tier 5 Server include all of the
    services listed in the Tier 5 column within this Midrange Service
    Description. Tier 5 Servers must be located in an HPE managed Data
    Center.MR036, and MR037).

## A.4 Phase Definitions

### Overview

A three-phase approach to creating a Run Book is now being implemented.

The three phases to a Run Book are:

1.  Infrastructure and Operating System (Infrastructure O/S Phase) –
    This is the initial rack/stack/cabling phase. The following types of
    configuration items are added and/or changed during this phase:

<!-- end list -->

  - > Virtual (VMs, Containers, LDOMs)

  - > Servers

  - > Blades

<!-- end list -->

6.  Application / Non Production – This phase is for the loading of
    binaries and application configuration.

7.  Production – This is the final Run Book being submitted and will
    take the server to production.

During the Application / Non Production and Production Phases, the
following types of configuration items may be included/modified :

  - > Middleware

  - > Database

  - > Application

### Run Book Sections

Every section of the Run Book template will include a table at the
beginning of the section indicating what actions are necessary in that
section of the Run Book. The table lists the possible actions.

| Action      | Identifier | Description                                                    |
| ----------- | ---------- | -------------------------------------------------------------- |
| Required    | R          | The section is required for the combination of Phase and Type. |
| Update      | U          | The section may need to be updated in the current phase.       |
| Required If | IF         | The section is required if the technology is being used.       |

The table at the beginning of each section is prefilled with the
required actions.

| Phase 1 - Infrastructure/OS | Phase 2 – Application Phase / Non Production | Phase 3 – Production |            |          |             |            |          |             |
| --------------------------- | -------------------------------------------- | -------------------- | ---------- | -------- | ----------- | ---------- | -------- | ----------- |
| Virtual                     | Server                                       | Blade                | Middleware | Database | Application | Middleware | Database | Application |
| R                           | R                                            | R                    | U          | U        | U           | U          | U        | U           |

