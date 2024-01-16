# Incident Report
---
> by *Tadiwanashe Shongedza*

## Issue Summary
---
In the afternoon of 15-07-2024 from 07:43 to 08:35 (Timezone: GMT+2), the ALX School Portal experienced a critical outage, rendering most user requests with `500 errors`. At its peak, 100% of users were unable to access essential features such as course materials and assignment submissions. The root cause was identified as a misconfiguration in the authentication service, leading to failed user authentication attempts and subsequent service disruption.

## Timeline
---
**Timezone:** [GMT+2]
**Outage Duration:** [07:43 - 08:35]
  - [07:43]: Abnormal server response times triggered monitoring alerts.
  - [07:45]: IT Support Team notified and initiated an investigation.
  - [07:50]: Initial assumption of heavy traffic or server load.
  - [07:55]: Network connectivity issues explored but ruled out.
  - [07:58]: Suspected cyberattack investigated, no evidence found.
  - [08:10]: Incident escalated to IT Support Team.
  - [08:16]: Root cause identified as misconfiguration in the authentication service.
  - [08:30]: Misconfiguration corrected, affected services restarted.
**Service Restored:** [08:35]

## Root cause
---
The root cause of the outage was a misconfiguration in the authentication service. Specifically, an incorrect setting in the authentication module prevented successful user authentication, leading to a cascade of failed requests and `500 errors`. The misconfiguration was likely introduced during recent updates to the portal's authentication system but remained undetected until the incident occurred.

## Resolution and Recovery
---
- [08:16]: Upon identification of the misconfiguration, the authentication service was immediately corrected to allow for successful user authentication.
- [08:30]: Affected services were restarted to apply the configuration changes.
- [08:35]: Service was restored, and users regained access to the School Portal.

## Corrective and Preventative Measures
---
- Regularly conduct thorough audits of configuration settings, especially after system updates or changes.
- Enhance monitoring for critical services, with specific alerts for authentication failures.
- Implement automated checks for critical configuration parameters, focusing on the authentication service.
- Review and update monitoring alerts and thresholds to ensure timely detection of anomalies.
- Document and communicate best practices for configuration management to relevant IT personnel.
- Schedule regular training sessions for IT staff to stay updated on incident response procedures and debugging techniques.

## Lessons Learned
---
Next time, we need to ensure more robust testing procedures after system updates to catch configuration issues early on. Additionally, clearer communication protocols need to be established for escalating and resolving critical incidents promptly.

