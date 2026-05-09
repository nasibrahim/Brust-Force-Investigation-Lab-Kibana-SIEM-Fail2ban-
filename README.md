Brute Force Investigation Lab (Kibana SIEM + Fail2ban)
Overview

This project demonstrates a basic SOC workflow using Kibana SIEM and Fail2ban to detect and respond to brute-force SSH login attempts on an Ubuntu Linux server.

The lab simulates repeated failed SSH authentication attempts and shows how security logs can be monitored, visualized, and automatically acted upon.

Objectives

Simulate SSH brute-force login attempts
Collect and monitor Linux authentication logs
Visualize attack activity in Kibana
Configure Fail2ban to automatically block malicious IPs
Perform basic incident investigation and reporting

Technologies Used
Ubuntu Linux
Kibana SIEM
Elastic Stack (ELK)
Fail2ban
SSH
Linux Authentication Logs

Lab Workflow:

Generate failed SSH login attempts
Ubuntu logs authentication failures
Logs are ingested into Kibana
Kibana visualizes brute-force activity
Fail2ban detects repeated failures
Malicious IP is automatically banned

Detection Results

Kibana Dashboard Findings
Multiple failed login attempts detected
Authentication failure patterns visualized
Event counts displayed through Kibana charts
Fail2ban Response
Suspicious IP automatically banned
SSH protection successfully triggered
Real-time defensive response implemented
Sample Fail2ban Output
sudo fail2ban-client status sshd

Output:

 Status for the jail: sshd
 Currently failed: 0
 Total failed: 5
 Currently banned: 1
 Total banned: 1
 Banned IP list: 192.169.10.1

Security Analysis

The attack pattern showed repeated failed login attempts targeting SSH services. Kibana SIEM successfully detected the abnormal activity through log monitoring and visualization, while Fail2ban mitigated the threat by banning the offending IP address automatically.

This project demonstrates:

Threat detection
Security monitoring
Automated response
Basic SOC investigation workflow

Skills Demonstrated:

SIEM Monitoring
Log Analysis
Linux Security
Threat Detection
Incident Investigation
Security Automation
Blue Team Operations


Nasiru Ibrahim
Aspiring SOC Analyst | Cybersecurity Enthusiast | SIEM & Linux Security Learner
