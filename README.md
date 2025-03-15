# SIEM-Based Log Analysis & Alert Tuning

## Objective

The SIEM-Based log analysis & alert tuning projecct aimed to set up a controlled environment and analyse the logs that is been generated by the multiple servers. The primary focuse was to ingest and analyse logs within the Security Information and Event Management (SIEM) system, configuring fleet to aggregate logs, creating custome dashboards in Kibana for real time monitoring and fine-tuning alert thresholds to reduse false positive.This hands-on experience enhanced understanding of log analysis, correlation rules, and improving threat detection accuracy.

### Skills Learned

- Proficiency in setting up and configuring SIEM tools like Kibana and Fleet for log collection and analysis.
- Ability to analyze security logs, identify anomalies, and detect potential threats.
- Fine-tuning alert thresholds to reduce false positives and improve threat detection accuracy.
- Creating custom dashboards in Kibana for real-time monitoring and data visualization.
- Strengthened ability to identify and respond to security incidents based on log insights.
- Understanding how to correlate logs from multiple sources to identify attack patterns and suspicious activity.
  
### Tools Used

- Kibana – For log analysis, visualization, and monitoring.
- Fleet – For collecting and managing logs from virtualy-hosted devices.
- Elasticsearch – For storing and indexing log data.
- Logstash – For processing and forwarding log data to Elasticsearch.
- VirtualBox- For hosting 2 servers(windows and ubuntu) and enabling log colecction

## Steps
**Steps Followed:**  

1. **Installed and Configured ELK Stack**  
   - Installed the ELK (Elasticsearch, Logstash, and Kibana) stack on the system to set up a centralized logging and monitoring       environment.  
   - Configured Elasticsearch as the backend for storing and indexing log data.  
   - Set up Logstash to collect, process, and forward log data to Elasticsearch.  
   - Installed and configured Kibana to visualize and analyze log data using customizable dashboards.  
   - Verified that all ELK components were running correctly and accessible.  

2. **Hosted Virtual Machines**  
   - Created two virtual machines (Windows and Ubuntu) using VirtualBox to simulate real-world network environments.  
   - Configured the network settings in VirtualBox to enable communication between the virtual machines and the ELK stack.  
   - Installed and configured necessary software on the virtual machines to generate system and security logs.  
   - Ensured that the virtual machines were running and connected to the network to enable log collection.  

3. **Configured Fleet for Centralized Log Collection**  
   - Installed the Elastic Agent on the virtual machines to enable log collection.  
   - Configured Fleet in Kibana to manage and monitor Elastic Agents.  
   - Connected the virtual machines to Fleet by enrolling the Elastic Agents.  
   - Set up policies in Fleet to define which logs to collect (e.g., system logs, authentication logs, security events).  
   - Verified that logs from the virtual machines were successfully being ingested into Elasticsearch.  

4. **Analyzed Logs**  
   - Used Kibana to explore and analyze logs collected from the virtual machines.  
   - Filtered logs based on source, type, and time to identify patterns and anomalies.  
   - Investigated security-related events such as failed logins, unauthorized access attempts, and system errors.  
   - Correlated logs from different sources to identify potential attack patterns and security threats.  

5. **Created Kibana Dashboards**  
   - Created multiple dashboards in Kibana to visualize different types of logs:  
     - **System Logs** – CPU usage, memory utilization, disk activity.  
     - **Authentication Logs** – Successful and failed login attempts.  
     - **Security Logs** – Unauthorized access attempts, firewall alerts.  
   - Configured charts, graphs, and tables in the dashboards for real-time monitoring and analysis.  
   - Ensured that dashboards provided a clear and comprehensive view of system health and security posture.  

6. **Fine-Tuned Alerts**  
   - Created alerting rules in Kibana to notify about critical events (e.g., multiple failed login attempts, unauthorized             access).  
   - Adjusted alert thresholds to reduce false positives and improve accuracy.  
   - Tested alerting rules by simulating attack scenarios and monitoring the response.  
   - Configured notification channels (e.g., email, Slack) to receive real-time alerts for critical events.  
   - Ensured that the alerts were actionable and provided sufficient context for incident response.  

### Conclusion

- Gained practical experience in setting up and managing a SIEM system using the ELK stack.
- Successfully hosted and monitored Windows and Ubuntu virtual machines for log collection.
- Configured Fleet to centralize log aggregation and management.
- Analyzed collected logs to identify patterns, anomalies, and security threats.
- Created custom Kibana dashboards for real-time monitoring and data visualization.
- Fine-tuned alert thresholds to improve detection accuracy and reduce false positives.
- Enhanced skills in log correlation, threat detection, and incident response.
