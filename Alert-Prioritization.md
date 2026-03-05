# Alert Priority Classification



In a SOC environment, alerts are prioritized based on impact, urgency, asset criticality, and exploit likelihood. Proper prioritization ensures that high-risk threats are handled first to minimize business impact.

###### 

###### Priority levels are defined as follows:



Critical: Active exploitation with severe business impact (e.g., ransomware, remote code execution on production systems).



High: Unauthorized access or confirmed malicious activity without immediate system-wide impact.



Medium: Suspicious activity requiring investigation but no confirmed compromise.



Low: Reconnaissance or benign activity with minimal risk.



##### Alert Prioritization Table

Alert Name	             CVSS Score	    Priority	            Reason for Priority

Ransomware Encryption Detected	9.8	Critical	Active file encryption causing service disruption

Log4Shell Exploit Attempt	9.8	Critical	Public exploit available, remote code execution risk

Unauthorized Admin Login	8.5	High     	Privilege escalation on critical system

Phishing Email Detected 	7.5	High	        Credential theft risk

Brute Force Login Attempts	6.5	Medium   	Multiple failures but no successful compromise

Port Scan Detected	        3.0	Low	        Reconnaissance activity only



###### Prioritization Criteria Used



###### Alerts were prioritized using the following criteria:



Asset Criticality: Production systems are prioritized higher than test or lab systems.



Exploit Likelihood: Known vulnerabilities with public exploits (e.g., Log4Shell) increase severity.



Business Impact: Potential financial loss, data breach, or service downtime.



Threat Activity: Active exploitation is treated with higher urgency than passive reconnaissance.



The CVSS score was used as a reference to quantify technical severity, while SOC context and business impact were used to finalize alert priority.



###### Outcome



This prioritization approach enables SOC analysts to focus on high-risk alerts first, reduce response time, and improve overall incident handling efficiency.
