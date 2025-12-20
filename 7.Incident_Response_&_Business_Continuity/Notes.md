# Incident Response and Business Continuity

- Business Continuity and Disaster Recovery Plan is important in every organization and environment.
- Mostly both Business Continuity and Disaster Recovery Plan ahave same document as they both complement each other but are not the same.
- Incident Response Plan have separate document.
- **Example: When a fire erupts**
  - **Incident Response Plan (IRP)**: Defines how to respond immediately to the fire when it occurs (e.g., evacuation, alerting emergency services, isolating affected areas).
  - **Disaster Recovery Plan (DRP)**: Explains how to recover or restore damaged materials, systems, or data after the fire
(e.g., restoring backups, repairing infrastructure).
  - **Business Continuity Plan (BCP)**: Describes how to keep the business running during and after the fire
(e.g., shifting operations to an alternate site, remote work).
- **Lateral Movement**: Technique used by attackers after gaining initial access to a system, where they move sideways within the internal network to access other systems, accounts, or sensitive data.
- **Case Study to Read**: [MGM Data Breach 2023](https://coursera-assessments.s3.amazonaws.com/assessments/1728158672868/8430c725-a8c6-496b-bd51-292b4fc51b45/Case%20Study-%20MGM%20Data%20Breach%202023.pdf)

## Incident Response Plan

- An Incident Response Plan (IRP) → Documented, structured approach that an organization follows to prepare for, detect, respond to, and recover from security incidents, such as cyberattacks, data breaches, malware infections, or system outages.
- Prepared in advance to clearly define how to respond when a security incident or attack occurs.
- It is proactive meaning it is created in advance before the incident.
- IRP is a detailed, documented plan for handling incidents.
- For **Reference**: [UnderDefense Incident Response Template](https://underdefense.com/incident-response-plan-template/)

### Roles in Incident Response

1. **Incident Response Manager/Team Lead**: Oversees the entire incident response process
2. **Security Analyst/Incident Handler**: Investigates and responds to incidents
3. **IT/System Administrator**: Handles technical systems and infrastructure
4. **Forensics Specialist**: Examines digital evidence
5. **Communications/PR Officer**: Manages internal and external communication
6. **Legal/Compliance Officer**: Ensures regulatory and legal obligations are met

### Phases of NIST Incident Response Lifecycle

<p align="center">
  <img src="https://github.com/user-attachments/assets/52e690d8-5aa2-4cbc-bdb5-b278d0d34024" alt="image" width="500" height="300" />
</p>

- There is no guidance for developing the Incident Response Plan but NIST shows the Lifecycle of Incident Response Plan.

#### 1. Preparation

- Identify critical systems and plan to protect them
- What to identify critical or not? It depends on the organization or company.
- Develop use cases and playbooks to define step-by-step actions for responding to different types of incidents or disasters.
- Use Cases → Describe scenarios of potential incidents and their impact.
- Playbooks → Step-by-step procedures to handle each scenario.

#### 2. Detection and Analysis

- Detect the incident and cause behind the incident.
- It can take time to detect the incident (e.g. The ransomware was in the computer for long time but detected it now).
- Note down the detection tools while detection and analysis.

#### 3. Containment, Eradication and Recovery

- **Containment**: Limiting the impact of the incident to prevent it from spreading further.
  - Purpose: Stop the attack or incident from affecting more systems or data.
  - Example: Isolating an infected computer from the network
- **Eradication**: Removing the root cause of the incident and eliminating any threats.
  - Purpose: Ensure the system is clean and the attacker or malware is removed.
  - Example: Deleting malware from infected systems
- **Recovery**: Restoring systems, data, and operations to normal functioning after the incident.
  - Purpose: Resume business and IT operations safely.
  - Example: Restoring data from backups
- Flow of the steps: Contain → Eradicate → Recover
- **Types of Containment**
1. **Short Term Containment**: Immediately stop the incident from spreading and limit damage.
   - Examples: Disconnecting an infected system from the network, Blocking a malicious IP address
2. **Long Term Containment**: Apply temporary but stable fixes so systems can operate safely until eradication and recovery are completed.
   - Examples: Applying temporary security patches, Moving services to a secure environment

#### 4. Post-Incident Activity

- Final phase where the organization reviews the incident after it has been resolved and uses the findings to improve future responses.
- After you stop the incident (containment), remove the cause (eradication), and restore systems (recovery), you then:
  - Analyze what went wrong
  - Identify why it happened
  - Document what was done
  - Improve policies, controls, and playbooks

## Disaster Recovery Plan

- A Disaster Recovery Plan (DRP) → Documented strategy that explains how an organization will restore critical systems, data, and IT operations after a major disruptive event, such as natural disasters, cyberattacks, hardware failures, or power outages.
- It is created before an incident to ensure quick recovery of IT systems after a disaster.
- It is proactive meaning it is created in advance before the incident.
- Disaster can be natural or man-made.
- **Redundant Server**: Backup or duplicate server that is deployed to take over operations if the primary server fails, ensuring high availability and business continuity.
  - If the primary server fails, the redundant server automatically or manually takes over
  - In **active–active** setups, data and traffic go to both servers. In **active–passive** setups, data is synchronized but traffic goes only to the main server until failover.
- Difference between **Data** and **Traffic**:
  - **Data**: Information that is stored or saved in systems.
    - Examples: Database records, Files and documents, User credentials, Logs and backups
    - Data must be stored, replicated, and backed up.
  - **Traffic**: The flow of requests and responses moving across a network.
    - Examples: User login requests, Website page requests, API calls, Network packets
    - Traffic is live and temporary.
- **Backup Server**: Server used to store copies of data from the primary system so that the data can be restored in case of data loss, corruption, or disaster.
  - Mainly focused on data protection, not live service availability.
  - Best practice is to keep backup servers on a separate network or isolated segment.
  - If a backup server must be on the same network, then:
    - It should be logically isolated (VLAN, firewall rules)
    - Access should be very limited
- Disaster recovery (DR) servers should ideally be far from the original (primary) servers.

## Business Continuity Plan

- A Business Continuity Plan (BCP) → Documented strategy that ensures critical business operations continue during and after a disruption or disaster.
- BCP is business-focused rather than IT-focused
- First, identify the systems that the business depends on and mark them as critical; then plan measures to ensure these systems continue operating even if a disaster occurs.
- Core Business Systems should continue for a long term even after the disaster
- Identify critical system by BIA (Business Impact Assessment)
- **Business Impact Assessment (BIA)**: Process used to identify and evaluate the effects of disruptions on critical business operations.
  - It helps an organization understand which processes and systems are most important and the potential impact if they fail.
- There is an ISO 22301 framework for the Business Continuity Management Systems (BCMS).

### RTO (Recovery Time Objective)

- **Meaning**: The maximum acceptable time it takes to restore a system or process after a disruption.
- In other words: how quickly you must recover to avoid serious business impact.
- **Example**: A casino’s slot machine system has an RTO of 4 hours → it must be back online within 4 hours after failure.

### RPO (Recovery Point Objective)

- **Meaning**: The maximum acceptable amount of data loss measured in time.
- In other words: how much data you can afford to lose in case of a disaster.
- **Example**: If the casino’s customer transaction database has an RPO of 1 hour, backups must ensure no more than 1 hour of data is lost.
