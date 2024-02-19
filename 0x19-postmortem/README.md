Issue Summary
- Duration: 
  - Start Time: February 18, 2024, 10:00 AM UTC
  - End Time: February 18, 2024, 1:00 PM UTC
- Impact: 
  - The web application's authentication service experienced a complete outage, rendering users unable to log in or access their accounts. Approximately 75% of users were affected, leading to a significant disruption in service.

Timeline:
- 10:15 AM UTC: Issue detected through monitoring alerts indicating a spike in failed login attempts.
- Actions taken:
  - Investigated backend authentication servers for any performance issues.
  - Checked network connectivity and load balancer configurations.
- Misleading investigation/debugging paths:
  - Initially suspected a database issue due to the high volume of failed login attempts, leading to unnecessary time spent on database diagnostics.
- Escalated the incident to the DevOps team at 10:45 AM UTC.
- Incident resolved by 1:00 PM UTC after identifying a misconfiguration in the firewall settings blocking traffic to the authentication servers.

Root Cause and Resolution
- Root Cause:
  - The outage was caused by a misconfiguration in the firewall rules, which inadvertently blocked incoming traffic to the authentication servers.
- Resolution:
  - The misconfigured firewall rules were identified and corrected promptly. Additionally, automated tests were implemented to ensure that firewall configurations align with the intended network traffic patterns.

Corrective and Preventative Measures
- Improvements/Fixes:
  - Implement stricter change management procedures for firewall configurations to prevent inadvertent misconfigurations.
  - Enhance monitoring and alerting systems to provide more granular visibility into authentication service performance and potential issues.
- Tasks:
  - Review and update firewall configuration documentation to ensure accuracy and completeness.
  - Conduct regular audits of firewall rules to identify and rectify any misconfigurations.
  - Implement automated tests to validate firewall rule changes before deployment.
  - Enhance incident response procedures to streamline escalation and resolution processes.

By implementing these measures, we aim to minimise the risk of similar outages in the future and ensure the continued reliability and availability of our web services.


