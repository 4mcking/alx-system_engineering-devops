# 0x19. Postmortem
Any software system will eventually fail, and that failure can come stem from a wide range of possible factors: bugs, traffic spikes, security issues, hardware failures, natural disasters, human error… Failing is normal and failing is actually a great opportunity to learn and improve. Any great Software Engineer must learn from his/her mistakes to make sure that they won’t happen again. Failing is fine, but failing twice because of the same issue is not.
Here is a postmortem 
# Issue Summary:
**Duration:** February 1st, 2023, 8:00 AM to 8:30 AM PST <br>
**Impact:** Our web-based application experienced a downtime of 30 minutes, affecting 100% of the users. During this time, users were unable to access the platform and experienced error messages. <br>
**Root Cause:** A misconfigured firewall rule blocked all incoming traffic to the web server.

# Timeline:
* **8:00 AM PST:** Issue detected - Monitoring alerts notified the engineering team of a significant drop in the number of requests being processed by the web server.
* **8:05 AM PST:** Investigation started - The on-call engineer started reviewing the logs and firewall rules to determine the root cause.
* **8:10 AM PST:** Misleading investigation - The initial assumption was that the issue was caused by a spike in traffic, leading the team to investigate the load balancing configuration.
* **8:15 AM PST:** Incident escalation - The incident was escalated to the lead engineer, who was able to quickly identify the misconfigured firewall rule.
* **8:30 AM PST:** Incident resolution - The misconfigured firewall rule was corrected, and the web server was restored to normal operations.

# Root Cause and Resolution:
The root cause of the outage was a misconfigured firewall rule that blocked all incoming traffic to the web server. During a recent security update, a new firewall rule was added to the system, but it was not properly tested before being deployed to production. This rule blocked all incoming traffic, including the requests to the web server, leading to the outage.
The issue was resolved by correcting the misconfigured firewall rule. The lead engineer was able to identify the issue and make the necessary changes to restore normal operations.

# Corrective and Preventative Measures:
* Improved testing procedures for firewall rules to ensure that they are properly tested before being deployed to production.
* Improved logging and monitoring to provide earlier detection of similar incidents in the future.
* Regular review of firewall rules to ensure that they are up-to-date and properly configured.

# Tasks:
* Implement improved testing procedures for firewall rules
* Enhance logging and monitoring for the web server
* Schedule regular reviews of firewall rules.


