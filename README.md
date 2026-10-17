# Digital Forensics & Incident Response Home Lab

### Building Practical Skills in Digital Forensic Examination, Cybercrime Investigation, and Incident Response

## Project Overview

Welcome to my Digital Forensics and Incident Response (DFIR) home lab.

This repository documents my transition from IT support and systems administration into the field of digital forensic examination and cybercrime investigation.

My professional background includes hands-on IT troubleshooting, Windows systems administration, networking, and cybersecurity fundamentals. I currently hold the following certifications:

- CompTIA A+
- CompTIA Network+
- CompTIA Security+
- AWS Certified Cloud Practitioner

My long-term career objective is to work as a digital forensic examiner or investigative technology specialist with a government agency, law enforcement organization, or government contractor.

I am particularly interested in supporting investigations involving human trafficking, child exploitation, cyberstalking, and other technology-facilitated crimes.

My background also includes graduate education in counseling psychology and previous professional experience in mental health and child protection. I hope to combine that understanding of human behavior and victim-centered work with technical investigative skills.

**This repository represents my ongoing learning and professional development, not completed professional forensic casework.**

---

## Lab Infrastructure

My home laboratory is built on a Dell PowerEdge T630 server running Proxmox Virtual Environment.

The lab provides a controlled environment for generating, preserving, examining, and documenting digital evidence.

### Virtual Machine Environment

| Virtual Machine | Operating System / Platform | Role |
|---|---|---|
| DFIR-Windows | Windows 11 | Dedicated forensic examination workstation |
| Victim-PC | Windows 11 | Controlled evidence-generation and investigation target |
| Windows Server | Windows Server with Active Directory | Domain authentication, account activity, and Windows security logging |
| Kali Linux | Kali Linux | Authorized security testing and controlled activity simulation |
| Security Onion | Linux-based security monitoring platform | Future network monitoring and incident investigation environment |

**Current configuration:** DFIR-Windows has 12 GB of allocated RAM, and Victim-PC has 4 GB. The Windows Server and Kali Linux VMs are part of the existing lab. Security Onion has been provisioned but is not yet operational.

### Planned Investigative Workflow

The laboratory is being developed around a repeatable investigative process:

1. Generate controlled activity on a Windows system.
2. Preserve and acquire relevant digital evidence.
3. Verify evidence integrity using cryptographic hashes.
4. Examine Windows and network artifacts.
5. Reconstruct a timeline of activity.
6. Correlate evidence across systems where appropriate.
7. Document findings in a structured investigative report.

All testing will be performed on systems I own or am authorized to use.

---

## Forensic Tools and Technologies

### Digital Forensic Examination

| Tool | Intended Purpose | Status |
|---|---|---|
| FTK Imager | Evidence acquisition, preview, and hash verification | Installation and initial setup |
| Autopsy | Disk and file-system forensic analysis | Planned |
| Eric Zimmerman's EZ Tools | Windows artifact parsing and timeline analysis | Planned |
| KAPE | Targeted Windows artifact collection and processing | Planned |
| Volatility | Memory forensic analysis | Future learning objective |

### Supporting Technologies

- **Proxmox VE:** Virtualization and laboratory management
- **Windows 11:** Host-based evidence generation and analysis
- **Windows Server / Active Directory:** Authentication and identity-related investigations
- **Kali Linux:** Controlled security testing
- **Git and GitHub:** Version control, documentation, and portfolio development

---

## Investigative Learning Objectives

### 1. Digital Evidence Acquisition and Preservation

Develop foundational skills in collecting and preserving digital evidence.

Topics include:

- Forensic disk imaging
- SHA-256 hash calculation and verification
- Evidence integrity
- Chain-of-custody documentation
- Working from verified copies of evidence
- Distinguishing live-response collection from offline acquisition

### 2. Windows Forensic Artifact Analysis

Learn to identify and interpret evidence left behind by Windows activity.

Artifacts of interest include:

- Windows Event Logs
- Windows Registry
- Prefetch
- Amcache and ShimCache
- LNK files and Jump Lists
- Browser history
- NTFS file-system metadata
- User account and logon activity

### 3. Active Directory Investigations

Use the Windows Server environment to understand how authentication and account activity can support an investigation.

Planned exercises include:

- Failed and successful authentication analysis
- Domain account changes
- Privileged account activity
- Windows security event correlation
- Investigating potentially unauthorized access

### 4. Controlled Security Simulations

Use Kali Linux to generate authorized activity within an isolated lab environment.

The objective is not simply to conduct security tests, but to understand what forensic evidence those activities leave behind.

Exercises will focus on identifying and reconstructing activity using host-based and, eventually, network-based evidence.

### 5. Network Forensics and Security Onion

Security Onion is a planned expansion once sufficient hardware resources are available and its configuration is completed.

Learning objectives include:

- Network traffic analysis
- Security alert investigation
- Network connection analysis
- Correlation of host and network evidence
- Incident timeline reconstruction

### 6. Investigative Documentation

Develop the ability to communicate technical findings clearly and objectively.

Each completed case study will aim to include:

- Investigation objective
- Scope and evidence sources
- Acquisition methodology
- Tools and versions
- Evidence integrity verification
- Analysis and findings
- Timeline of relevant events
- Limitations and unresolved questions
- Lessons learned

---

## Planned Forensic Case Studies

### Case 001 — Windows Workstation Activity Investigation

**Status: Planned**

Scenario: A Windows 11 workstation is suspected of unauthorized activity.

Objectives:

- Acquire and preserve a forensic copy of the evidence.
- Examine relevant Windows artifacts.
- Identify user and application activity.
- Develop a timeline of events.
- Produce an introductory forensic examination report.

### Case 002 — Active Directory Authentication Investigation

**Status: Planned**

Scenario: Unusual authentication activity is detected within a small Windows domain.

Objectives:

- Review domain controller security logs.
- Identify relevant authentication events.
- Correlate domain activity with workstation evidence.
- Determine which conclusions the available evidence supports.
- Document findings and investigative limitations.

### Case 003 — Network and Host Evidence Correlation

**Status: Future Project**

Scenario: Controlled suspicious network activity occurs within the laboratory.

Objectives:

- Generate authorized test activity.
- Collect relevant network telemetry.
- Examine corresponding Windows artifacts.
- Correlate network and host observations.
- Reconstruct an incident timeline.

This project will be developed after Security Onion is operational.

---

## Project Progress

### Phase 1 — Laboratory Construction

- [x] Establish Proxmox virtualization environment
- [x] Deploy Windows 11 forensic workstation
- [x] Deploy Windows 11 victim workstation
- [x] Configure VM memory and virtual hardware
- [x] Establish Windows Server / Active Directory VM
- [x] Establish Kali Linux VM
- [x] Create public GitHub repository
- [ ] Publish lab architecture diagram
- [ ] Complete forensic workstation tool configuration

### Phase 2 — Foundational Digital Forensics

- [ ] Complete first forensic evidence acquisition
- [ ] Calculate and verify evidence hashes
- [ ] Analyze introductory Windows artifacts
- [ ] Build an investigation timeline
- [ ] Publish first forensic case study

### Phase 3 — Expanded Investigations

- [ ] Complete Active Directory investigation
- [ ] Introduce controlled security-testing scenarios
- [ ] Configure Security Onion
- [ ] Correlate host and network evidence
- [ ] Develop additional documented case studies

---

## Professional Development and Career Objectives

I am developing this laboratory as part of a longer-term transition into digital forensic examination and investigative technology.

My areas of professional interest include:

- Digital forensic examination
- Cybercrime investigation
- Criminal intelligence and investigative analysis
- Technology-facilitated exploitation investigations
- Evidence preservation and investigative reporting
- Victim-centered investigative support

I am interested in connecting with digital forensic examiners, cybercrime investigators, intelligence analysts, and professionals working in government or law enforcement support roles.

I welcome constructive feedback on my laboratory, investigative methodology, documentation, and professional development.

---

## Evidence Handling and Ethical Considerations

This repository is intended for educational and professional development purposes.

- All simulated investigations will use authorized systems and controlled or appropriately licensed training evidence.
- No actual victim data, personal identifying information, credentials, or sensitive investigative evidence will be published.
- Evidence integrity, repeatability, and accurate documentation are central learning objectives.
- Investigative findings will distinguish observed facts from interpretations and assumptions.
- All exercises will be conducted within appropriate legal and ethical boundaries.

---

## Repository Roadmap

As the project develops, this repository will contain:

- Lab architecture diagrams and configuration documentation
- Forensic tool installation and usage notes
- Windows artifact analysis exercises
- Sanitized screenshots
- Case studies and investigation reports
- Lessons learned and technical references

This repository will evolve as I gain experience, complete training, and develop stronger investigative skills.

---

*Project initiated: October 2026*

*Purpose: Hands-on education, technical skill development, and preparation for a career in digital forensic examination.*
