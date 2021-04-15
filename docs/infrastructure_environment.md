# Infrastructure Environment

***\[**This section contains a description of the environment in which the application will operate and* *should be completed by AA or a designated third-party technology provider in conjunction with the hosting provider.*

*In the case of technical deployments which involve virtualization technologies please refer to the Data Center Zoned Virtual Machine Resource Allocation Policy maintained by the AA Landing Zone owner.**\]*** 

## Hardware Information    

### Virtual Server (VM)/VMWare Windows/Linux

| Phase 1 - Infrastructure/OS | Phase 2 – Application Phase / Non Production | Phase 3 – Production |            |          |             |            |          |             |
| --------------------------- | -------------------------------------------- | -------------------- | ---------- | -------- | ----------- | ---------- | -------- | ----------- |
| Virtual                     | Server                                       | Blade                | Middleware | Database | Application | Middleware | Database | Application |
| R                           |                                              |                      | U          | U        | U           |            |          |             |

**Virtual server information is to be provided by AA or designatedthird-party technology provider.**
**If the project will exist on virtual servers that are considered “shared services” the virtual server specifications can be obtained from the ITS Project Manager or Technologist. Otherwise if the project will exist on dedicated equipment the virtual server specifications can be obtained from the Bill of Materials.**

**Note: A Virtual Server Information Sheet must be completed for each managed instance in the project. Please copy and add additional Virtual Server Information Sheets as needed.**

| Distributed Resource Scheduler Rules | Provide DRS rules here, for example keep apappp39/40 separate. |
| ------------------------------------ | -------------------------------------------------------------- |
|                                      |                                                                |

| **Virtual Server (VM)/Zone Information Sheet** |                                                             |                           |                                                           |
|------------------------------------------------|-------------------------------------------------------------|---------------------------|-----------------------------------------------------------|
| VM Name                                        | server1         | Landing Zone              | N/A  |
| OS Version and Service Pack                    | Linux Ubuntu 19.04      | Production Tier Level     | N/A     |
| Deployment Type                                | Template | Pre-Production Tier Level | Tier-1: Development |
| VM Domain                                      | test2.com          | VM OU                     | N/A            |
| AA IT Vertical                                 | N/A        | Cost Center               | 1234   |
| FQDN                                           | N/A            |                           |                                                           |

| **Resources**         |                                                              |                         |                                                                 |
|-----------------------|--------------------------------------------------------------|-------------------------|-----------------------------------------------------------------|
| VM Config             | Medium Standard       |                         |                                                                 |
| CPU: vCPU             | N/A             | Memory: vMEM (GB)       | N/A             |
| CPU (Mhz) Reservation | N/A | Memory (MB) Reservation | N/A | 
| **Network**                            |                    |                     |               |             |
|----------------------------------------|--------------------|---------------------|---------------|-------------|
| **NIC Devices**                        | **Color Zone**     | **vLAN ID**         | **IP/CIDR**   | **Gateway** |
| 1234 | Yellow | N/A | 123.123.123.123 | 255.255.255.0 | 

| **Storage**                |                         |                                                |                 |               |
|----------------------------|-------------------------|------------------------------------------------|-----------------|---------------|
| **Disk (SCSI Controller)** | **OS - Disk Size (GB)** | **Storage Tier – VMDK Provision**              | **Mount point** | **Size (GB)** | 
| Hard Disk 1 (vSCSI 0:0)    | Windows / 60 GB         | Tier 1/Tier 3/Tier Gold : Thin/Thick Lazy Zero | C:              | 60GB          |
| Hard Disk 1 (vSCSI 0:0)    | RHEL 7.x / 40 GB        |                                                | /               | 6GB           |
|                            |                         |                                                | swap            | 4GB           |
|                            |                         |                                                | /tmp            | 2GB           |
|                            |                         |                                                | /boot           | 500MB         |
|                            |                         |                                                | /var            | 6GB           |
|                            |                         |                                                | /usr            | 8GB           |
|                            |                         |                                                | /home           | 2GB           |
|                            |                         |                                                | /var/crash      | 8GB           |
| Hard Disk 2 (vSCSI 0:1)    | Windows / 40 GB         |                                                | D:              | 40GB          |
| Hard Disk 2 (vSCSI 0:1)    | RHEL 7.x / 30 GB        |                                                | /opt            | 30GB          | 

| **Additional Customization/Optional VM Info** |                                                                       |               |                                                |
|-----------------------------------------------|-----------------------------------------------------------------------|---------------|------------------------------------------------|
| VM Maintenance Window                         | N/A        | Temp Password | Do not document any passwords in the Run Book. |
| System Login Name                             | N/A          | Temp Password | Do not document any passwords in the Run Book. |
| App Login Name                                | N/A          |               |                                                |
| Installed software                            | N/A |               |                                                |  

## IHS WebServer Information

| Phase 1 - Infrastructure/OS | Phase 2 – Application Phase / Non Production | Phase 3 – Production |            |          |             |            |          |             |
| --------------------------- | -------------------------------------------- | -------------------- | ---------- | -------- | ----------- | ---------- | -------- | ----------- |
| Virtual                     | Server                                       | Blade                | Middleware | Database | Application | Middleware | Database | Application |
|                             |                                              |                      | IF         |          |             |            |          |             |

***\[**Optional: Use only if WebServer is required. If this information
is not required, type “N/A” in the heading line, “Not applicable to this
project” here, and delete the table.**\]***

| Web Server Information                                                                    | Comments/Example                            |
|-------------------------------------------------------------------------------------------|---------------------------------------------|
| Web Server Release                                                                        | 9.0        |
| Environments needed                                                                       | Stage    |
| How much traffic is expected? Hits per sec? Concurrent users?                             | N/A        |
| Are there expected peak hours for higher transactions? Daily, monthly, quarterly, yearly? | N/A    |
| If Any what % of Growth are you expecting over 6 months, 1, 3, years?                     | N/A         |
| Additional agents/services needed                                                         | N/A |
| If using WebLogic proxy plugin what IP’s and ports will the JVM’s be using?               | N/A |
| What type of Content?                                                                     | N/A        |
| Are there any authentication requirements?                                                | No |
| Archive log requirement                                                                   | access        |
| Backup Needs                                                                              | NO         |       

     

### Virtual Server (VM)/VMWare Windows/Linux

| Phase 1 - Infrastructure/OS | Phase 2 – Application Phase / Non Production | Phase 3 – Production |            |          |             |            |          |             |
| --------------------------- | -------------------------------------------- | -------------------- | ---------- | -------- | ----------- | ---------- | -------- | ----------- |
| Virtual                     | Server                                       | Blade                | Middleware | Database | Application | Middleware | Database | Application |
| R                           |                                              |                      | U          | U        | U           |            |          |             |

**Virtual server information is to be provided by AA or designatedthird-party technology provider.**
**If the project will exist on virtual servers that are considered “shared services” the virtual server specifications can be obtained from the ITS Project Manager or Technologist. Otherwise if the project will exist on dedicated equipment the virtual server specifications can be obtained from the Bill of Materials.**

**Note: A Virtual Server Information Sheet must be completed for each managed instance in the project. Please copy and add additional Virtual Server Information Sheets as needed.**

| Distributed Resource Scheduler Rules | Provide DRS rules here, for example keep apappp39/40 separate. |
| ------------------------------------ | -------------------------------------------------------------- |
|                                      |                                                                |

| **Virtual Server (VM)/Zone Information Sheet** |                                                             |                           |                                                           |
|------------------------------------------------|-------------------------------------------------------------|---------------------------|-----------------------------------------------------------|
| VM Name                                        | server2         | Landing Zone              | N/A  |
| OS Version and Service Pack                    | Linux Ubuntu 19.04      | Production Tier Level     | N/A     |
| Deployment Type                                | Template | Pre-Production Tier Level | Tier-1: Development |
| VM Domain                                      | test2.com          | VM OU                     | N/A            |
| AA IT Vertical                                 | N/A        | Cost Center               | 1234   |
| FQDN                                           | N/A            |                           |                                                           |

| **Resources**         |                                                              |                         |                                                                 |
|-----------------------|--------------------------------------------------------------|-------------------------|-----------------------------------------------------------------|
| VM Config             | Medium Standard       |                         |                                                                 |
| CPU: vCPU             | N/A             | Memory: vMEM (GB)       | N/A             |
| CPU (Mhz) Reservation | N/A | Memory (MB) Reservation | N/A | 
| **Network**                            |                    |                     |               |             |
|----------------------------------------|--------------------|---------------------|---------------|-------------|
| **NIC Devices**                        | **Color Zone**     | **vLAN ID**         | **IP/CIDR**   | **Gateway** |
| 1234 | Yellow | N/A | 123.123.123.124 | 255.255.255.0 | 

| **Storage**                |                         |                                                |                 |               |
|----------------------------|-------------------------|------------------------------------------------|-----------------|---------------|
| **Disk (SCSI Controller)** | **OS - Disk Size (GB)** | **Storage Tier – VMDK Provision**              | **Mount point** | **Size (GB)** | 
| Hard Disk 1 (vSCSI 0:0)    | Windows / 60 GB         | Tier 1/Tier 3/Tier Gold : Thin/Thick Lazy Zero | C:              | 60GB          |
| Hard Disk 1 (vSCSI 0:0)    | RHEL 7.x / 40 GB        |                                                | /               | 6GB           |
|                            |                         |                                                | swap            | 4GB           |
|                            |                         |                                                | /tmp            | 2GB           |
|                            |                         |                                                | /boot           | 500MB         |
|                            |                         |                                                | /var            | 6GB           |
|                            |                         |                                                | /usr            | 8GB           |
|                            |                         |                                                | /home           | 2GB           |
|                            |                         |                                                | /var/crash      | 8GB           |
| Hard Disk 2 (vSCSI 0:1)    | Windows / 40 GB         |                                                | D:              | 40GB          |
| Hard Disk 2 (vSCSI 0:1)    | RHEL 7.x / 30 GB        |                                                | /opt            | 30GB          | 

| **Additional Customization/Optional VM Info** |                                                                       |               |                                                |
|-----------------------------------------------|-----------------------------------------------------------------------|---------------|------------------------------------------------|
| VM Maintenance Window                         | N/A        | Temp Password | Do not document any passwords in the Run Book. |
| System Login Name                             | N/A          | Temp Password | Do not document any passwords in the Run Book. |
| App Login Name                                | N/A          |               |                                                |
| Installed software                            | N/A |               |                                                |   

## WebSphere Information

| Phase 1 - Infrastructure/OS | Phase 2 – Application Phase / Non Production | Phase 3 – Production |            |          |             |            |          |             |
| --------------------------- | -------------------------------------------- | -------------------- | ---------- | -------- | ----------- | ---------- | -------- | ----------- |
| Virtual                     | Server                                       | Blade                | Middleware | Database | Application | Middleware | Database | Application |
|                             |                                              |                      | IF         |          |             |            |          |             |

***\[**Optional - Use only if J2EE Servers are required. If this information is not required, type “N/A” in the heading line, “Not applicable to this project” here, and delete the table.**\]***

| WebLogic/WebSphere Information                                                   | Comments/Example                             |
|----------------------------------------------------------------------------------|----------------------------------------------|
| WebLogic/WebSphere Version and Service Pack                                      | 9.0         |
| Number of JVM/Node Required                                                      | 2 per node            |
| Log rotation required                                                            | NO    |
| WebLogic/WebSphere Application Server Directory                                  | /opt/was90       |
| Environments needed                                                              | Stage     |
| Clustering Required                                                              | NO      |
| Virtual IP bound to J2EE server                                                  | N/A      |
| WebLogic / WebSphere Configuration                                               | N/A |
| Create Application specific USER/Password – OS or LDAP based                     | N/A            |
| What is the backend Database                                                     | N/A      |
| Does application server require any Database Client installation for connection? | N/A       |
| Specify monitoring requirements                                                  | N/A      |
| Archive log requirement                                                          | N/A         |      

       

## Device Network Information Request

| Phase 1 - Infrastructure/OS | Phase 2 – Application Phase / Non Production | Phase 3 – Production |            |          |             |            |          |             |
| --------------------------- | -------------------------------------------- | -------------------- | ---------- | -------- | ----------- | ---------- | -------- | ----------- |
| Virtual                     | Server                                       | Blade                | Middleware | Database | Application | Middleware | Database | Application |
| R                           | R                                            | R                    |            |          |             |            |          |             |

(Cabling and ECN information Worksheet)

***\[**AA ITS Network provides a full Network ECN to the service provider unless AA requests that it be developed by the service provider. The abbreviated ECNM for local connectivity shall be included here or by reference to an attached spreadsheet document. This information will be used in server and application implementations and support and the cable request form.**\]***


### Engineering Cable Diagram

| Phase 1 - Infrastructure/OS | Phase 2 – Application Phase / Non Production | Phase 3 – Production |            |          |             |            |          |             |
| --------------------------- | -------------------------------------------- | -------------------- | ---------- | -------- | ----------- | ---------- | -------- | ----------- |
| Virtual                     | Server                                       | Blade                | Middleware | Database | Application | Middleware | Database | Application |
|                             | R                                            |                      |            |          |             |            |          |             |

***\[**A cable diagram for local connectivity shall be included here or by reference to an attached document. This visual diagram will be used to assist the implementation team with expected connections and their location on the server. This may be an HP-required diagram.**\]***

This diagram is *required* for new hardware. 
## BigIP Configuration Information 

| Phase 1 - Infrastructure/OS | Phase 2 – Application Phase / Non Production | Phase 3 – Production |            |          |             |            |          |             |
| --------------------------- | -------------------------------------------- | -------------------- | ---------- | -------- | ----------- | ---------- | -------- | ----------- |
| Virtual                     | Server                                       | Blade                | Middleware | Database | Application | Middleware | Database | Application |
|                             |                                              |                      | R          | R        | R           | U          | U        | U           |

***\[**BigIP information to be provided by AA or designated third-party technology provider**\]**.*

BigIP information for both Stage and Production is copied directly from the approved BigIP forms and includes information such as the following:

### Stage 

### Production 

 
| SSL Certificates |
|------------------|
| apptest.com | 

 
| Health Monitors |
|-----------------|
| hm1 | 

 

 
| Profiles |
|----------|
| profile1 | 

 

 

 
| Virtual Servers |
|-----------------|
| vs1 | 

   

## DNS Guidelines

| Phase 1 - Infrastructure/OS | Phase 2 – Application Phase / Non Production | Phase 3 – Production |            |          |             |            |          |             |
| --------------------------- | -------------------------------------------- | -------------------- | ---------- | -------- | ----------- | ---------- | -------- | ----------- |
| Virtual                     | Server                                       | Blade                | Middleware | Database | Application | Middleware | Database | Application |
|                             |                                              |                      | R          | R        | R           | R          | R        | R           |

***\[**This may be an HPE-specific requirement.**\]*** 
Each system should be configured to use these DNS servers. The order of precedence is determined by deployment location. The file to update on Unix servers is /etc/resolv.conf

**For servers in CDC**:

1. 10.61.134.5 (AADNS2)
2. 10.58.134.5 (AADNS1)

**For servers in Plano**

1. 10.61.134.5 (AADNS2)
2. 10.58.134.5 (AADNS1)

**For servers at HDQ**

1. 10.58.134.5 (AADNS1)
2. 10.61.134.5 (AADNS2)

**For servers at CENTURY LINK TECHNOLOGY SOLUTIONS**

1. 10.61.134.5 (AADNS2)
2. 10.58.134.5 (AADNS1)