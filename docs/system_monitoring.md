# System Monitoring

***\[**To be completed by AA or designated Applications Team supporting the software running on the specified servers contained in this Run Book.**\]***

**\*\*NOTE: HPE will apply OS specific monitoring to each server. This baseline will monitor items such as CPU, swap, native OS filesystems etc. Monitoring requirements for tools or applications installed after the OS will need to be documented below. For questions about HPE Global Standards please contact the HPE CSR.**     

## UNIX Monitoring

### Processes 

| Phase 1 - Infrastructure/OS | Phase 2 – Application Phase / Non Production | Phase 3 – Production |            |          |             |            |          |             |
| --------------------------- | -------------------------------------------- | -------------------- | ---------- | -------- | ----------- | ---------- | -------- | ----------- |
| Virtual                     | Server                                       | Blade                | Middleware | Database | Application | Middleware | Database | Application |
|                             |                                              |                      | IF         | IF       | IF          |            |          | IF          |

***\[**Use the output from the ps command to determine the Process path, Process Name, Command Line arguments, and Process Owner field. The Proc Min is the minimum number of instances that must be running at all times. The Proc Max is the maximum number of instances that must be running at all times.**\]***

| Server Name | Process Path | Process Name | Command Line Arguments | Proc Min | Proc Max | Process Owner | Procedure Number |
| ----------- | ------------ | ------------ | ---------------------- | -------- | -------- | ------------- | ---------------- |
| server1 | /opt/ihs90 | httpd | N/A | N/A | N/A | root | 1 |
| server2 | /opt/was90 | java | N/A | N/A | N/A | root | 2 |








### File Systems

| Phase 1 - Infrastructure/OS | Phase 2 – Application Phase / Non Production | Phase 3 – Production |            |          |             |            |          |             |
| --------------------------- | -------------------------------------------- | -------------------- | ---------- | -------- | ----------- | ---------- | -------- | ----------- |
| Virtual                     | Server                                       | Blade                | Middleware | Database | Application | Middleware | Database | Application |
|                             |                                              |                      | IF         | IF       | IF          |            |          | IF          |

The Monitor (Yes/No) is used to determine if MRC should monitor this file system or not. This needs to be completed for EVERY mounted file system on the server that is not a Standard Monitored mounted file system. \*\*NOTE: Threshold value for % full will trigger a file system space alert when the threshold is crossed (+1%).

| Server Name | File System | Clustered FileSystem (Y/N) | Critical Threshold (% Full) | Monitor (Yes/No) | Procedure Number |
| ----------- | ----------- | -------------------------- | --------------------------- | ---------------- | ---------------- |
| server2 | /opt/was90 | N/A | 85 | Yes | 3 |  

## URL Monitoring


| URL (http/https) | Check for specific error messages | Retrieve detailed download information | HTTP server response | Frequency of the check | Alert Procedure |
|------------------|-----------------------------------|----------------------------------------|----------------------|------------------------|-----------------|
| apptest.com | N/A | N/A | 200 | 5min | 4 |

## Alert Procedures


| Procedure Number | Actions |
|------------------|---------|
| 1 | Call WebTeam |
| 2 | Call WebTeam |
| 3 | Call Unix team and WebTeam |
| 4 | call WebTeam and networking | 