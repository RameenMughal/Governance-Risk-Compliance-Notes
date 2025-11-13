# Policies Concept

## Understanding Policy

- **Rule** -> Mandatory to do
- **Policy**
  - Statements to achieve specific goal.
  - Set of ideas or plans that is used for making decisions, especially in politics, economics or businesses.
  - Mostly in management team so the this team needs to be serious about Information Security.
  - Policy needs to be specific (e.g. Encryption should be applied for privacy then specify what encryption method like AES)
- **Policy in GRC**
  - Formal statement of intent or rule that guides decisions and behavior within an organization.
  - In GRC, policies are the foundation for ensuring governance consistency, risk management, and compliance with laws or standards (e.g. ISO 27001, NIST, GDPR).
- Then rules are made after policy to achieve that goal.
- Example -> The policy is to make data private so the rule will be enforced like one employee cannot use another employee's computer.
- Flat Network
  - Everything is connected together with no barriers.
  - No VLANs
  - There should not be a flat network in organization as it has risk (attacker can cause malware to come in and organization's network will be compromised).
  - There should be different networks among organizations like divided in departments.
- **Difference between Policy and Framework?**
  - Policy
    - Set of mandatory rules or principles that defines the goals and desired outcomes.
    - Policy tells how the GRC will be implemented.
  - Framework
    - Provides the structure, tools and guidance for implementing those policies.
    - Frameworks guides how the GRC should be.
- **Examples of Policy**
  - Information Security Policy -> Defines how data should be protected
  - Access Control Policy -> Defines user access rights and responsibilities
  - Incident Response Policy -> Defines how to react to security incidents
  - Data Protection and Privacy Policy -> Classify what data needs to be protected
- **Procdure**
  - A procedure is a step-by-step description of how to implement or comply with a policy.
  - It turns the policy into actionable tasks.

## Policy Lifecycle

The Policy Lifecycle outlines the stages a policy goes through from creation to maintenance.  

It ensures that policies are effectively developed, communicated, managed, and reviewed.

<img width="500" height="400" alt="image" src="https://github.com/user-attachments/assets/83cd7fc0-ff63-4608-92ac-14aa9249eaa7" />

### **1. Creation**
Defines the initial steps of policy development.

- **Need:** Identify why the policy is required.  
- **Ownership:** Assign responsibility for creating and maintaining the policy.  
- **Writing:** Draft the policy with clear, concise, and compliant language.  
- **Approval:** Obtain necessary approvals from management or governing bodies.

### **2. Communication**
Ensures awareness and understanding of the policy across the organization.

- **Publication:** Distribute the policy through official channels (e.g. published through Internal Memo in organization) 
- **Training:** Educate employees or stakeholders about policy details and compliance.  
- **Attestation:** Confirm that individuals have read and acknowledged the policy.

### **3. Management**
Focuses on policy enforcement and handling exceptions.

- **Enforcement:** Monitor compliance and ensure adherence to the policy by clarifying rules.  
- **Exception Management:** Handle and record situations where the policy cannot be followed.

### **4. Maintenance**
Keeps policies up-to-date and relevant.

- **Review:** Periodically evaluate the policy’s effectiveness and accuracy.  
- **Archival:** Retire outdated policies while maintaining historical records.

**Goal:** Maintain a continuous cycle of improvement and compliance throughout the policy’s life.

## Writing Policy

- **Important in Writing Policy**
  - Purpose
  - Scope
  - Roles and Responsibilities
  - Exceptions
- **Scenario**: Small Fintech Company
- **Data Classification Policy** -> How the data is stored and classified by severity
- **Purpose** -> The purpose is to make sure all data is classified and handled as per it's sensitivity, to maintain the CIA triad and adhere to the regulatory requirements
- Password will not be inlcuded in Data Classification as it has it's own policy named Password Management Policy
- **Scope**
  - Employees
  - All types of data (electronic, paper and verbal communication)
  - Third party vendor
  - All systems (applications, database and cloud).
- **Roles and Responsibilities**
  1. Employee -> Handle data as per the assigned classification
  2. Data Owner -> Classify the data correctly
  3. Data Custodian -> Handles how to store data correctly
  4. GRC Officer -> Complied as per policy
- Data Owner is one the most important people in organization that knows the data.
- Data Custodian then implements the data and classifies
- If data is not correctly classified then Data Custodian is responsible for this.
- **Policy Statements**
  1. Data must be classified as per it's sensitivity
  2. Data should be classified based on pre-defined levels
     - Public -> Approved for public view then **low** severity
     - Internal -> Intended for internal use then **medium** severity
     - Confidential -> Sensitive information that may cause harm if leaked then **high** severity
  3. Data should be stored with backups or should be disposed when not in use.
- **Exceptions** -> If there is an exception, it should be formally approved by the Head of Department.

## Task: Policy Development

**Objective:** You will demonstrate your understanding of GRC by developing, context appropriate information security policies tailored to a specific industry.

**Industry Options:** You must choose one industry:
1. Pharmaceuticals: protecting clinical trial data, research IP, and patient records.
2. Retail: securing customer data, payment systems, and vendor access.
3. Aviation: protecting flight systems, passenger data, and operational technologies.

**Task Description:**
You are part of an organization’s information security team. Your task is to design a policy set to
ensure the protection of data, systems, and compliance obligations within your chosen
industry. You must:
1. Identify key risks specific to your chosen sector.
2. Draft a concise but complete security policy addressing critical areas (examples below).
3. Include a short justification paragraph for each policy explaining why it’s needed in your
context.
4. Ensure the tone, structure, and terminology reflect professional GRC standards.
5. You may use any format or template, as long as it’s consistent and readable.

Choose any policy (Access Management Policy, Data Protection & Privacy Policy and more).
