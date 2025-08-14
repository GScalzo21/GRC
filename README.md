# Corporate Cybersecurity Assessment Utilizing NIST Cybersecurity Framework (CSF) 2.0  

## Introduction  

For this project, I stepped into the role of assessing an organization’s cybersecurity posture — in this case, **Oscorp** — and designing a full program to lift them toward compliance with the [NIST CSF 2.0](https://www.nist.gov/publications/nist-cybersecurity-framework-csf-20).  

Think of it like a real engagement: I was given a “current state” snapshot that mimicked the type of report you’d get after initial interviews and a round of fact-finding. From there, I ran Oscorp through the CSF lens, marking them on a pass/fail basis and building a roadmap to close the gaps.  

I kicked things off with a short, high-level presentation to stakeholders — the kind of session where you don’t bury people in jargon, but you help them see where the organization stands and where it needs to go. From there, I built out the heavy-hitting piece: a set of concrete recommendations and actionable procedures designed to move Oscorp from reactive to adaptive.  

![horizon_labs2](https://github.com/user-attachments/assets/6e1c3012-8e1f-4351-8bcc-3889bf7498a3)  

## CSF Core Functions  
The CSF Core Functions — **GOVERN, IDENTIFY, PROTECT, DETECT, RESPOND, and RECOVER** — act like the backbone of the framework. They break cybersecurity down into outcomes you can actually measure and improve on.  

| Core Functions  | Description |
| --------------- | ----- |
| ![Screenshot 2024-10-28 134244](https://github.com/user-attachments/assets/c536c78f-b8d2-4988-a1ad-ea1b0222bd41) | Establishing and enforcing the organization’s cybersecurity risk strategy, expectations, and policies. |
| ![Screenshot 2024-10-28 134430](https://github.com/user-attachments/assets/bd218bc5-9048-4d91-96fd-77aba367d87b) | Understanding the current risks and where the organization stands. |
| ![Screenshot 2024-10-28 134438](https://github.com/user-attachments/assets/f6554061-0d01-49e9-91df-b102eb4b8ac7) | Putting safeguards in place to reduce those risks. |
| ![Screenshot 2024-10-28 134447](https://github.com/user-attachments/assets/26e591c9-9ee6-454f-9f5b-37062bec1d0c) | Detecting and analyzing potential threats before they spiral. |
| ![Screenshot 2024-10-28 134456](https://github.com/user-attachments/assets/bfdf2e21-ced1-4767-8ac6-4ec982b6f5e3) | Acting quickly and effectively once an incident is identified. |
| ![Screenshot 2024-10-28 134503](https://github.com/user-attachments/assets/10ef5d64-da8b-41df-a0fe-56acb244fd1c) | Recovering assets and operations post-incident, minimizing downtime and damage. |

---

<!-- GOVERN -->  
![Screenshot 2024-10-28 135023](https://github.com/user-attachments/assets/a9b93ba7-a2a2-4cdc-954f-8016f3df6e58)  

When we talk governance, we’re talking about how seriously an organization takes cybersecurity at the top. NIST CSF 2.0 lays out tiers that let you measure this maturity.  

![image](https://github.com/user-attachments/assets/60704a33-4b7f-4925-8eef-4084d5fa484c)  

A **Current Profile** shows you where the organization stands right now — what outcomes they’re hitting, how they’re being achieved (or not achieved), and whether the approach is structured or scattered.  

👉 **Oscorp’s current profile landed at Tier 1: Partial.**  

| Tier           | Cybersecurity Risk Governance      | Cybersecurity Risk Management |
|---------------|------------------------------------|------------------------------|
| Tier 1: Partial | Risk strategy exists in theory but is applied inconsistently. Prioritization is ad hoc, not tied to clear objectives or threat intel. | Awareness of risk is low across the org. Risk management is one-off and reactionary. Cybersecurity info isn’t widely shared internally, and supplier-related risks aren’t really on the radar. |

A **Target Profile** is where the organization wants to be — where leadership sets its sights, based on what’s coming down the pipeline (new tech, customer demands, regulatory shifts, threat trends).  

👉 **For Oscorp, the goal was Tier 4: Adaptive.**  

| Tier           | Cybersecurity Risk Governance | Cybersecurity Risk Management |
|---------------|-------------------------------|------------------------------|
| Tier 4: Adaptive | Risk management is baked into strategy and culture. Executives treat cyber risk the same way they treat financial risk. Budgets are shaped around risk realities. Cybersecurity is part of everyday decision-making, not an afterthought. | The org continuously learns from past incidents, adapts quickly to new threats, and uses real-time intel to drive decisions. Risks tied to suppliers and third parties are monitored constantly. Security knowledge flows across the company and to trusted partners. |

Throughout this process, one lens never leaves the table: the **CIA Triad** — keeping data **Confidential**, ensuring its **Integrity**, and making it **Available** when needed. Every weakness or blind spot ultimately ties back to one of those three pillars.  
![image](https://github.com/user-attachments/assets/5b8e35de-2c04-4de8-a82c-bb526a3f6f5c)

---

<details close> 
<summary> <h3> Oscorp's Current Status Report (Click to expand)</h3> </summary>

**Current Cybersecurity Team:**
- Cybersecurity Analyst: A generalist who reacts to incidents as they happen. Reports to the IT Manager.  
- Network Engineer: Maintains firewalls. Reports to the Network Team Lead.  
- Cybersecurity Consultant: That’s me. Brought in to bring structure, reporting initially to the IT Manager.  

**Current Security Controls in Place:**

- **Organizational Governance:**  
  - Business strategy exists at the CEO level, but cybersecurity strategy does not.  
  - Roles and responsibilities for security are loosely handed off to IT.  

- **Asset Management:**  
  - A basic spreadsheet tracks laptops with serial numbers, models, and warranties.  
  - All apps are SaaS-based, with data sitting in Microsoft Azure.  
  - Microsoft Office 365 powers productivity.  
  - IT uses a Secure Operating Environment (SOE) to image laptops with Windows.  

- **Business Continuity & Disaster Recovery:**  
  - Documented business continuity plan is in place.  
  - Regular disaster recovery tests are conducted.  
  - Backups happen consistently and get tested.  

- **Vulnerability Management:**  
  - Oscorp owns Qualys but only runs scans on an ad-hoc basis.  
  - No structured vulnerability management program exists.  
  - As a result, a pile of high/severe vulnerabilities remain unresolved.  

- **Risk Management:**  
  - There’s a risk team, but they only focus on financial risks.  
  - No cyber or technology risk processes are active.  

- **Third-Party Risk:**  
  - Procurement and finance review contracts, but IT/security is not involved.  
  - No structured third-party/vendor risk process exists.  

- **Identity & Access Management (IAM):**  
  - Microsoft Active Directory manages users and groups.  
  - No privileged access management solution in place.  
  - Shared admin accounts among senior IT staff.  
  - Access is granted by request, without strong governance.  
  - No two-factor authentication in use.  
  - Passwords are “complex,” but that’s the only safeguard.  
  - Remote access handled by VPN.  

- **Network Security:**  
  - Palo Alto Next Gen firewalls in place.  
  - Firewalls get annual audits and regular updates.  
  - Network diagrams (including cloud) are up to date.  
  - VLANs segment the network.  

- **Physical Security:**  
  - Strongest area so far — CCTV, vetting, and 24/7 monitoring are all in place.  

- **Data Security:**  
  - No Data Loss Prevention (DLP) solution.  
  - All sensitive data resides in Azure and Office 365.  
  - A critical SaaS application runs out of Horizon Labs.  

- **Policy:**  
  - One generic IT policy.  
  - No formal security policy, no data governance, no classification standards.  

- **Detection & Response:**  
  - No SIEM, no proactive detection.  
  - Security response is limited to AV alerts from Microsoft Defender.  

- **Security Awareness & Training:**  
  - A one-time induction module with very basic cybersecurity training.  
  - No ongoing awareness campaigns.  

</details>

---

## Assessment Kickoff

Using the CSF Core Functions as a guide, Oscorp’s current environment shows **serious gaps across multiple domains**.  

Some areas (like physical security and basic business continuity planning) are in decent shape. But cyber risk governance, IAM, vulnerability management, and detection/response are all underdeveloped or outright missing.  

Recommendations will follow each subcategory in later sections, mapped back to the CSF outcomes.  

---
<!--IDENTIFY-->
![Screenshot 2024-10-28 134831](https://github.com/user-attachments/assets/9dc5bda1-08f0-4d90-b806-34621a19553a)

---

<details close> 
<summary> <h3> NIST Cybersecurity Framework 2.0 Pass/Fail Logs (Click here)</h3> </summary>

![Screenshot 2024-10-27 205100](https://github.com/user-attachments/assets/586dd539-f042-4bea-b9d2-290b8e445571)  

![Screenshot 2024-10-27 205255](https://github.com/user-attachments/assets/c0c4e42a-7736-48b1-ac59-92604fef17ca)

</details>

---

### Asset Management
- *Devices are tracked, but no IP addresses or agents are tied to them.* This kills the effectiveness of vulnerability scans because the scanner can’t authenticate.  
- *Third-party systems are not catalogued.* Contracts are tracked, but IT/security isn’t even in the loop.  
- *Resources are not classified by sensitivity or business value.* No labeling, no prioritization.  
- *Cybersecurity roles and responsibilities across employees and vendors are undefined.*  

**Recommendations:**  
- Implement a **formal vulnerability management policy** that classifies and prioritizes findings.  
- Deploy **scanning agents** on all network-connected assets (permanent and non-permanent) to widen coverage.  
- Launch a **third-party risk program** with IT directly involved in vendor assessments.  
- Classify assets by sensitivity/criticality using a **Maximum Tolerable Outage (MTO) matrix**.  

![image](https://github.com/user-attachments/assets/0fd3f160-1f11-4da1-a781-d0837b1115c7)  
*(RPO = Recovery Point Objective, RTO = Recovery Time Objective, WRT = Work Recovery Time)*  

---

### Business Environment
- *Oscorp doesn’t have a documented role in its supply chain.*  

**Recommendations:**  
- Create clear documentation of Oscorp’s **role in the supply chain**.  
- Map suppliers, then classify them by **criticality and sensitivity** to ensure high-risk vendors get more scrutiny.  

---

### Governance
- *No organizational information security policy.*  
- *No documented or assigned security roles internally or externally.*  
- *No regulatory or legal requirements around cyber/privacy documented.*  
- *No governance or oversight process for cybersecurity risk.*  

**Recommendations:**  
- Draft and enforce a **formal Cyber & Information Security Policy**.  
- Define and document **roles and responsibilities** across IT, leadership, and vendors.  
- Capture and manage **legal/regulatory requirements** that apply to Oscorp.  
- Establish a **governance structure** with board-level visibility and oversight of security risks.  

---

### Risk Assessment & Risk Management Strategy
- *Vulnerabilities aren’t tracked or documented. Scans are random at best.*  
- *No external threat intel feeds or forums being used.*  
- *No threat modeling or business impact assessments.*  
- *Risk tolerance hasn’t been defined or communicated.*  

**Recommendations:**  
- Stand up a **full Cybersecurity Risk Management Policy**.  
- Align with **OWASP Secure Design Principles** and validate against **NIST 800-53 controls**.  
- Document risks using a **Risk Matrix** (likelihood vs. impact) to set tolerance levels.  
- Identify and categorize both **tangible and intangible assets**, then tie them into the risk framework.  

![Screenshot 2024-09-06 155149](https://github.com/user-attachments/assets/88309da8-792e-4e3d-a6ed-d7c293cfc655)

---

<!--PROTECT-->
![Screenshot 2024-10-28 134843](https://github.com/user-attachments/assets/eaa0f70b-acb1-43ba-9186-53f4c406875c)

---

<details close> 
<summary> <h3> NIST Cybersecurity Framework 2.0 Pass/Fail Logs (Click here)</h3> </summary>

![Screenshot 2024-10-28 141833](https://github.com/user-attachments/assets/83ff0872-74e1-4969-a1f2-29a639abb176)  

![Screenshot 2024-10-28 142000](https://github.com/user-attachments/assets/f36bc530-31e3-4425-a67d-2a70586aa605)  

![Screenshot 2024-10-28 142028](https://github.com/user-attachments/assets/cac40a40-e19a-464c-a819-e8f1651e5231)

</details>

---

### Access Controls
- *Identities and credentials are unmanaged.* No MFA, no regular reviews, no offboarding process.  
- *Physical access isn’t managed beyond basic security.* No logs, no biometrics, no entry/exit validation.  
- *Remote access lacks strong authentication.* VPN has no MFA.  
- *Permissions are handed out without least privilege or separation of duties.*  

**Recommendations:**  
- Roll out a full **Identity & Access Management (IAM) policy**.  
- Enforce **Multi-Factor Authentication (MFA)** for all accounts and VPN.  
- Implement **role-based access control (RBAC)** and **access control lists (ACLs)**.  
- Standardize **onboarding/offboarding** with periodic access reviews.  
- Strengthen **remote access policies** with mandatory 2FA.  

---

### Awareness Training
- *Users are left in the dark.* No onboarding, no refreshers, and no process to verify whether training actually sticks.  
- *Privileged users don’t grasp their extra responsibilities.* No PAM (Privileged Access Management) or specific guidance in place.  
- *Third-party partners, suppliers, and even customers aren’t briefed on security expectations.*  
- *Executives and board members aren’t trained on security risks or decision-making responsibilities.*  
- *Physical security staff and IT have no clear role definitions tied to cybersecurity.*  

**Recommendations:**  
- Build and roll out a **formal Training & Education program** that runs periodically, stays current, and is measured for effectiveness.  
- Extend training to **third-party providers** through the TPRM (Third-Party Risk Management) program.  
- Stand up **executive/board-specific awareness sessions**.  
- Define **roles and responsibilities** across employees, IT, execs, vendors, and physical security staff.  

---

### Data Security
- *Data-at-rest isn’t classified or labeled.* Azure is storing it, but without tagging, it’s just a bucket of risk.  
- *Data-in-transit has no guardrails.* No USB controls, no monitoring, no encryption protocols enforced.  
- *Asset lifecycle isn’t managed.* No policies for how data or devices are offboarded, transferred, or destroyed.  
- *No DLP (Data Loss Prevention) strategy exists.*  

**Recommendations:**  
- Implement a **Data Loss Prevention program**.  
- Classify and label data properly so DLP can be effective.  
- Monitor **USB transfers and exfiltration attempts**.  
- Create and enforce **data/asset disposal policies**.  

---

### Information Protection Processes & Procedures
- *No change management process.* Configuration changes happen ad-hoc with no tracking.  
- *Physical environment protections exist, but there’s no written policy.*  
- *Data destruction isn’t standardized or audited.*  
- *Protection tech effectiveness isn’t shared internally.*  
- *HR practices lack deprovisioning and personnel screening.*  
- *Vulnerability scans happen randomly, but no actual program exists.*  

**Recommendations:**  
- Create a **formal Change Management policy** and enforce it.  
- Define and document **physical security policies**.  
- Roll out a **data disposal process** aligned with regulatory requirements.  
- Establish **HR-driven onboarding and offboarding protocols**.  
- Stand up a **formal Vulnerability Management plan** with scheduled scans and clear remediation workflows.  

---

### Protective Technology
- *No event or log management.* No SIEM, no reviews, nothing.  
- *Removable media is wide open.* USBs can move data freely with no policy.  
- *Network traffic isn’t properly monitored.* No detection of anomalies or command-and-control behavior.  

**Recommendations:**  
- Deploy a **Security Information & Event Management (SIEM)** platform. Align monitoring with **MITRE ATT&CK** for visibility.  
- Write and enforce **removable media and data exfiltration policies**.  
- Expand **network monitoring capabilities** beyond default Microsoft Defender alerts.  

---

<!--## DETECT-->
![Screenshot 2024-10-28 134853](https://github.com/user-attachments/assets/2a5d2bd2-ba9b-4cff-84c2-840f73c4633b)

<details close> 
<summary> <h3> NIST Cybersecurity Framework 2.0 Pass/Fail Logs (Click here)</h3> </summary>

![Screenshot 2024-10-28 142453](https://github.com/user-attachments/assets/e8f4d360-6015-451c-8484-3fc6b868b63b)  
![Screenshot 2024-10-28 142508](https://github.com/user-attachments/assets/7fc2cbd1-0dcd-4818-8413-c17ef30d0716)

</details>

---

### Anomalies and Events
- Deploy a **SIEM** to capture and monitor logs and network traffic.  
- Establish event classification (**low/medium/high**) and escalation paths.  
- Train analysts on threat analysis and root cause investigation.  

### Security Continuous Monitoring
- Expand beyond Microsoft Defender-only alerts.  
- Define **scope of monitoring**, detection thresholds, and escalation.  
- Build **detection and response playbooks**.  
- Extend monitoring to third-party risk and vendor ecosystems.  
- Run **scheduled vulnerability scans** with remediation tracking.  

### Detection Processes
- Define **roles and responsibilities** between IT and security.  
- Enforce **separation of duties** where appropriate.  
- Conduct **regular penetration tests** to validate controls.  

---

<!-- RESPOND-->
![Screenshot 2024-10-28 134902](https://github.com/user-attachments/assets/0e5fa430-0cea-4d22-be43-912381a82917)

<details close> 
<summary> <h3> NIST Cybersecurity Framework 2.0 Pass/Fail Logs (Click here)</h3> </summary>

![Screenshot 2024-10-28 142705](https://github.com/user-attachments/assets/ef22e6a8-8635-47a4-abfc-80181246c01c)

</details>

---

### Response Planning
- Draft and implement a **formal Incident Response Plan**.  

### Communications
- Define **internal and external communications protocols** during incidents.  
- Include escalation contacts, regulators, vendors, and industry peers.  
- Document thresholds for when law enforcement must be contacted.  

### Analysis
- Ensure incidents are **analyzed for root cause and criticality**.  
- Retain ability to support **forensic investigations**.  

### Mitigation
- Base response plans on **SANS IR Framework**.  
- Build a **Vulnerability Management Program** to quickly handle new, known, and zero-day threats.  
- Test containment strategies periodically.  

### Improvements
- Regularly **test, refine, and improve IR plans**.  
- Run **tabletop exercises** and simulations.  

---

<!--## RECOVER-->
![Screenshot 2024-10-28 134912](https://github.com/user-attachments/assets/b595cac7-1881-4388-b3ac-4e5f59a099fc)

<details close> 
<summary> <h3> NIST Cybersecurity Framework 2.0 Pass/Fail Logs (Click here)</h3> </summary>

![Screenshot 2024-10-28 142747](https://github.com/user-attachments/assets/92ba5adc-b78e-447e-bba8-c2d2103bdefc)

</details>

---

### Communications
- Coordinate recovery efforts with **vendors, ISPs, incident response partners, and CSIRTs**.  
- Build a **reputation recovery strategy** to handle brand and trust impact post-incident.  

---

## Conclusion
After investigating Oscorp’s security posture, I mapped findings to the **NIST CSF 2.0**. I pulled in additional frameworks like **MITRE ATT&CK, NIST 800-53, and OWASP Secure Design Principles** to shape a roadmap for a stronger, more resilient cybersecurity program. The end goal: helping Oscorp evolve from *reactive firefighting* to a **proactive, auditable, and certifiable security posture**.  


