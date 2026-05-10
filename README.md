SSH Brute-Force Detection & Mitigation Using Kibana SIEM and Fail2ban

Overview

This project demonstrates the detection, investigation, and automated mitigation of SSH brute-force activity within an Ubuntu Linux environment using Kibana SIEM and Fail2ban.

The environment was configured to monitor Linux authentication events, visualize suspicious login activity, and automatically respond to repeated authentication failures.

---

Security Investigation Summary

During monitoring activities, Kibana SIEM identified multiple failed SSH authentication attempts targeting the server.

Key Findings

- 10 failed SSH login attempts detected through Kibana dashboards
- Authentication logs revealed repeated access attempts against the SSH service
- Attack activity originated from a single IP source
- Fail2ban automatically banned the offending IP after exceeding the configured failure threshold

---

Technologies Used

- Ubuntu Linux
- Elastic Stack (ELK)
- Kibana SIEM
- Fail2ban
- SSH
- Linux Authentication Logs

---

Detection & Response Workflow

. SSH authentication failures generated security events
. Ubuntu system logs recorded the failed login attempts
. Logs were ingested into Kibana SIEM
. Kibana visualized authentication failure patterns and event counts
. Fail2ban continuously monitored authentication logs
. Automatic IP blocking was triggered after repeated failed attempts

---

Investigation Results

Kibana SIEM

- Visualized authentication failure trends
- Displayed event distribution for failed SSH logins
- Enabled centralized monitoring and investigation of security events

Fail2ban

- Detected repeated failed login attempts
- Automatically banned the suspicious IP address
- Reduced exposure to continued brute-force activity

---

Security Outcome

The environment successfully demonstrated:

- Centralized log monitoring
- Authentication event analysis
- Brute-force detection
- Automated incident response
- Linux security monitoring

The integration of Kibana SIEM and Fail2ban provided both visibility and active mitigation against suspicious SSH authentication activity.

---

Author

Nasiru Ibrahim
SOC Analyst | Cybersecurity Enthusiast | SIEM & Linux Security Operation
