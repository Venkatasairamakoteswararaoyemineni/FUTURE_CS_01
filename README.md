# FUTURE_CS_01
________________________________________

README – Vulnerability Assessment of a Live Web Application

📌 Project Overview

This project documents a comprehensive vulnerability assessment performed on the live test site testaspnet.vulnweb.com using the industry standard tool OWASP ZAP (v2.17.0 by Checkmarx).

The assessment followed recognized methodologies including the OWASP Testing Guide v4 and NIST SP 800 115, ensuring a structured, reliable, and repeatable 
evaluation process.

The primary objective was to:

•	Identify potential security weaknesses.

•	Analyze their severity using CVSS v3.1 scoring.

•	Provide practical remediation strategies to strengthen the application’s security posture.
________________________________________
🔍 Scope

•	Target URLs:

o	http://testaspnet.vulnweb.com

o	https://testaspnet.vulnweb.com

________________________________________

•	Methodology:

o	Reconnaissance & Information Gathering

o	Automated Scanning with OWASP ZAP

o	Manual Verification of Findings

o	CVSS v3.1 Risk Scoring

o	Reporting & Remediation Planning
________________________________________
📊 Findings Summary

A total of 14 vulnerabilities were identified:

•	Medium (4)

o	Absence of Anti CSRF Tokens

o	Missing Content Security Policy (CSP) Header

o	Missing Anti Clickjacking Header

o	HTTP only site (no HTTPS enforcement)

________________________________________

•	Low (5)

o	Cookie without SameSite attribute

o	X Powered By header leak

o	Server version disclosure

o	X AspNet Version header leak

o	Missing X Content Type Options header

________________________________________

•	Informational (5)

o	Minor observations such as verbose error messages and unnecessary HTTP methods.
________________________________________
📈 Visuals

•	Pie Chart: Distribution of vulnerabilities (4 Medium, 5 Low, 5 Informational).

•	Bar Chart: CVSS v3.1 scores for each vulnerability.

•	Flow Diagram: Configuration weaknesses mapped to potential attack vectors (CSRF, clickjacking, session hijacking).
________________________________________
🛠 Recommendations

•	Implement missing security headers (CSP, X Frame Options, HSTS, X Content Type Options).

•	Enforce HTTPS with a valid SSL/TLS certificate.

•	Strengthen cookie policies (HttpOnly, Secure, SameSite).

•	Suppress or genericize server headers to reduce information leakage.

•	Re scan after remediation to validate fixes.
________________________________________
🎯 Skills Demonstrated

•	Web Application Security Testing

•	Vulnerability Analysis & Risk Assessment

•	Application of Security Standards (OWASP, NIST)

•	Professional Reporting & Remediation Planning
________________________________________
✅ Conclusion

This project highlights the importance of proactive security testing. While no critical vulnerabilities were found, the identified configuration weaknesses 
represent potential risks if left unresolved. By applying the recommended fixes, the application can achieve a stronger security posture without major redesigns.
________________________________________
