# VAPT Fundamentals

- VAPT (Vulnerability Assessment and Penetration Testing)
  - Identifies and exploits weakness in systems, networks or applications.
  - Goal -> Find vulnerabilities before attackers do.
  - Make your mind like an attacker.

- VA (Vulnerability Assessment)
  - Output file of VA -> Risk Report.
  - Broad Coverage like it checks all the IP addresses of the network.

- PT (Penetration Testing)
  - Output of PT -> Proof of Exploit.
  - Deap and focused on one specific thing.

- Core Concepts
  - Scope Definition -> Define what to do.
  - Rules of Engagement (RoE) -> Written permission (don't to PT without permission as it will be considered illegal).
  - Testing Types -> Black, Grey or White Box.

- Cyber Kill Chain -> Core Concept of VAPT
  - Reconnaissance -> Information Gathering.
  - Weaponization -> Uses above information gathered to create malicious payload.
  - Delivery -> Execute the payload in the target's system.
  - Exploitation -> Payload activated to gain access to the target's system.
  - Installation -> Install malware or backdoors into the target's system to gain access completely (can access the system again without exploiting again).
  - Command & Control (C2 or C&C) -> Establish communication with the system to maintain control and issue further commands.
  - Actions on Objectives -> What was the main purpose of exploiting the system.

- LFI (Local File Inclusion) -> Web Application Vulnerability that lets an attacker trick the site into opening files from the server.
- Post Exploitation Phase comes from Actions on Objectives in Cyber Kill Chain

## Demonstration of Nmap Command
- Virtual Machine - Metasploitable
- Nmap -> Port Scanning Tool
- `nmap MACHINE_IP` -> Gives all open ports and their types like `80/tcp open http`
- `nmap -sV MACHINE_IP` -> Gives versions of the systems running on all open ports like `80/tcp  open  http  Apache httpd 2.4.46`
- First Nmap was only port scanning but now it is also used for exploitation as the tool is advanced

## Relationship Between VAPT and GRC
- VAPT identifies the technical risk
  - VAPT is like the detective.
  - It finds vulnerabilities (e.g., SQL injection, weak password, open ports).
  - It also provides a technical severity — like Low, Medium, High, Critical — based on how easily the issue could be exploited.

- GRC evaluates the business impact
  - GRC takes the VAPT finding and asks:
  - “If this vulnerability were exploited, how would it affect our business operations, reputation, or compliance?”
  - GRC assigns a business impact level — like financial loss, reputational damage, data breach consequences, etc.

- VAPT = confirms the risk is real and exploitable.
- GRC = calculates how much that risk matters to the organization.

-------------------------------------------------------------------------------------------------------------

- CVE (Common Vulnerabilities Exposure) -> New ID for New Vulnerability
- Common Vulnerabilities in Websites
  - SQL Injection
  - RCE (Remote Control Execution)
  - XSS (Cross Site Scripting)
- Reporting and Documentation in VAPT
  - Vulnerability Description
  - Overview and Explanation how the vulnerability was exploited.
  - Define Severity and Impact
  - PoC (Proof of Concept) -> Code or steps that you used to exploit the vulnerability
  - Recommendations to solve the problem.
