# <span style="color:#38BDF8; font-family:Trebuchet MS;">Real-Time SIEM Monitoring and Intrusion Detection System</span>

---

# <span style="color:#38BDF8; font-family:Trebuchet MS;">Project Overview</span>

This project demonstrates a **Real-Time Security Information and Event Management (SIEM)** implementation designed to monitor, detect, analyze, and visualize cyberattacks in a controlled cybersecurity lab environment.

The implementation integrates:

- Attack simulation
- Intrusion detection
- Centralized log collection
- Security event correlation
- Real-time alert monitoring
- SOC-style dashboard visualization

The project was implemented using:

- **Kali Linux** – Attacker Machine
- **DVWA** – Vulnerable Web Application
- **Snort IDS** – Intrusion Detection System
- **Wazuh SIEM** – Centralized Monitoring Platform

---

# <span style="color:#38BDF8; font-family:Trebuchet MS;">SIEM Architecture Workflow</span>

1. **Kali Linux** performs cyberattacks against the vulnerable server.
2. **DVWA** acts as the target vulnerable application.
3. **Snort IDS** monitors network traffic and detects malicious activities.
4. **Wazuh SIEM** collects logs and correlates security events.
5. **Wazuh Dashboard** displays real-time alerts and monitoring data.

---

# <span style="color:#38BDF8; font-family:Trebuchet MS;">1. Attacker Machine – Kali Linux</span>

Kali Linux was configured as the attacker environment to simulate real-world cyberattacks.

## <span style="color:#38BDF8; font-family:Georgia;">Activities Performed</span>

### Vulnerability Scanning
- Identified open ports, running services, and vulnerabilities.

### SQL Injection Attacks
- Tested backend database vulnerabilities using malicious SQL queries.

### Brute-Force Login Attempts
- Performed repeated login attempts to gain unauthorized access.

### Directory Enumeration
- Scanned hidden directories and files on the web server.

### Web Application Exploitation
- Exploited insecure DVWA modules for testing purposes.

### Packet Generation for IDS Monitoring
- Generated malicious traffic for Snort IDS analysis.

## <span style="color:#38BDF8; font-family:Georgia;">Purpose</span>

- Simulate attacker behavior and generate malicious traffic for monitoring.

---

# <span style="color:#38BDF8; font-family:Trebuchet MS;">2. Target Server – DVWA Vulnerable Web Application</span>

DVWA was deployed as the intentionally vulnerable target application.

## <span style="color:#38BDF8; font-family:Georgia;">Implementation Activities</span>

### DVWA Deployment
- Hosted DVWA on Apache web server.

### Vulnerable Module Configuration
- Enabled insecure modules for penetration testing.

### Logging Integration
- Configured logging mechanisms for monitoring activities.

### Traffic Forwarding
- Forwarded traffic to Snort IDS for packet inspection.

## <span style="color:#38BDF8; font-family:Georgia;">Purpose</span>

- Provide a vulnerable environment for cybersecurity testing.

---

# <span style="color:#38BDF8; font-family:Trebuchet MS;">3. Snort IDS – Intrusion Detection System</span>

Snort IDS was used to inspect network traffic and detect suspicious activities in real time.

## <span style="color:#38BDF8; font-family:Georgia;">Detection Functions</span>

### Real-Time Packet Inspection
- Monitored live network packets continuously.

### Signature-Based Detection
- Matched packets against predefined attack signatures.

### Traffic Monitoring
- Analyzed incoming and outgoing communications.

### Rule-Based Alert Generation
- Generated alerts for suspicious activities.

### Malicious Payload Detection
- Identified malicious payloads inside packets.

---

## <span style="color:#38BDF8; font-family:Georgia;">Detection Examples</span>

### SQL Injection Detection
- Detected malicious SQL query patterns.

### Port Scan Detection
- Identified reconnaissance scanning attempts.

### Brute-Force Detection
- Detected repeated failed login attempts.

### Suspicious HTTP Request Detection
- Monitored abnormal web requests.

### Unauthorized Access Detection
- Identified attempts to access restricted resources.

## <span style="color:#38BDF8; font-family:Georgia;">Purpose</span>

- Detect attacks and generate intrusion alerts in real time.

---

# <span style="color:#38BDF8; font-family:Trebuchet MS;">4. Wazuh SIEM Platform</span>

Wazuh SIEM acted as the centralized monitoring and log management platform.

## <span style="color:#38BDF8; font-family:Georgia;">Key Functionalities</span>

### Centralized Log Management
- Collected logs from servers and security devices.

### Security Event Correlation
- Correlated related security events for analysis.

### Real-Time Alert Monitoring
- Displayed live security alerts instantly.

### Threat Visualization Dashboard
- Visualized attack patterns and incidents.

### Incident Tracking
- Tracked detected security incidents.

### Alert Severity Classification
- Categorized alerts based on severity levels.

---

## <span style="color:#38BDF8; font-family:Georgia;">Log Sources</span>

### Snort IDS Alerts
- Intrusion alerts generated by Snort IDS.

### Apache Access Logs
- Recorded web server requests and activities.

### System Authentication Logs
- Monitored login and authentication events.

### Web Application Activity Logs
- Logged DVWA user activities and attack attempts.

## <span style="color:#38BDF8; font-family:Georgia;">Purpose</span>

- Provide centralized visibility and security event analysis.

---

# <span style="color:#38BDF8; font-family:Trebuchet MS;">5. Wazuh Dashboard</span>

The Wazuh Dashboard provided a graphical interface for monitoring alerts and incidents.

## <span style="color:#38BDF8; font-family:Georgia;">Dashboard Monitoring Included</span>

### Live Attack Alerts
- Displayed real-time intrusion alerts.

### Event Severity Levels
- Classified alerts based on criticality.

### Log Analytics
- Analyzed logs for suspicious trends.

### Source IP Tracking
- Identified attacker IP addresses.

### Attack Timelines
- Visualized attack sequences and timestamps.

### Security Event Visualization
- Presented incidents using charts and dashboards.

## <span style="color:#38BDF8; font-family:Georgia;">Purpose</span>

- Enable SOC-style security monitoring and incident investigation.

---

# <span style="color:#38BDF8; font-family:Trebuchet MS;">Complete Workflow Lifecycle</span>

## Phase 1 – Environment Setup
- Configured virtual cybersecurity lab
- Installed Kali Linux attacker machine
- Deployed DVWA vulnerable application
- Installed Snort IDS
- Configured Wazuh SIEM and dashboard

---

## Phase 2 – Attack Simulation
- Kali Linux launched cyberattacks against DVWA
- Malicious traffic passed through monitored network
- Attack packets reached the target server

---

## Phase 3 – Intrusion Detection
- Snort inspected packets in real time
- IDS rules matched malicious patterns
- Intrusion alerts were generated

---

## Phase 4 – Log Collection and Correlation
- Wazuh collected logs from Snort and servers
- SIEM engine correlated related events
- Alerts classified based on severity

---

## Phase 5 – Real-Time Monitoring
- Wazuh Dashboard displayed live alerts
- SOC-style visualization enabled attack analysis
- Security events monitored continuously

---

# <span style="color:#38BDF8; font-family:Trebuchet MS;">Technologies and Tools Used</span>

## Kali Linux
- Penetration testing operating system for attack simulation.

## DVWA
- Vulnerable web application for cybersecurity testing.

## Snort IDS
- Open-source intrusion detection system for traffic monitoring.

## Wazuh SIEM
- Centralized SIEM platform for log analysis and monitoring.

## Apache Server
- Web server hosting the DVWA application.

## Linux
- Operating system environment for deployment.

## Virtual Machines
- Isolated environment for cybersecurity experimentation.

---

# <span style="color:#38BDF8; font-family:Trebuchet MS;">Skills Gained</span>

## SIEM Monitoring
- Learned centralized security monitoring and alert analysis.

## Intrusion Detection
- Implemented IDS-based threat detection techniques.

## Log Analysis
- Analyzed logs to identify malicious activities.

## Threat Detection
- Detected suspicious activities using SIEM and IDS tools.

## SOC Operations
- Understood Security Operations Center workflows.

## Incident Investigation
- Investigated alerts and validated suspicious events.

## Network Security
- Monitored abnormal network traffic patterns.

## Cyberattack Simulation
- Performed controlled attack simulations in a lab environment.

---

# <span style="color:#38BDF8; font-family:Trebuchet MS;">Project Outcome</span>

The project successfully demonstrated a real-time SIEM monitoring architecture capable of:

- Detecting cyberattacks
- Monitoring suspicious activities
- Correlating security events
- Visualizing incidents in real time
- Simulating SOC monitoring workflows

This implementation provided practical hands-on experience in:

- SIEM Monitoring
- Intrusion Detection
- Log Analysis
- Threat Detection
- Incident Response
- Security Operations Center (SOC) workflows

---

# <span style="color:#38BDF8; font-family:Trebuchet MS;">Future Enhancements</span>

- Integrate Suricata IDS
- Add automated incident response
- Configure email alert notifications
- Implement threat intelligence feeds
- Add machine learning-based anomaly detection

---

# <span style="color:#38BDF8; font-family:Trebuchet MS;">Author</span>

**Sivananthan M**  
Cybersecurity Enthusiast | SIEM Monitoring | SOC Operations | Threat Detection
