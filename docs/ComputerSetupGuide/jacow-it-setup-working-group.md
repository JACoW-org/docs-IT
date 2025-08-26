# IT Setup Working Group

![header](./figures/header.png "header logo")
*Contributors: IT Setup Working Group Members*  
*Page contact: Ivan Andrian (Elettra-Sincrotrone Trieste S.C.p.A.)*  
*Last update: Unknown*

---

At this Working Group both experts and newcomers meet and discuss the current status of the IT setup for JACoW conferences.

## Mission Statement

The aim is to share the JACoW experience, best practices, identify possible weaknesses and envisage any improvement.

---

## Current Technology Status

### Present Software Environment

| Component | Current Status |
|-----------|----------------|
| **Operating System** | Windows 10 |
| **Office Suite** | Office 2016-2019 |
| **PDF Processing** | Acrobat 12 or 2017 DC |

### Setup and Deployment Evolution

#### Legacy Approaches - Status
- **Virtual machines (2016 idea):** Probably not practical or sustainable
- **JACoW Software bundle:** Over, unmaintained
- **Traditional cloning:** May no longer be necessary

#### Modern Approach - Under Investigation
- **Bootstrap tool investigation:** [Chocolatey](https://chocolatey.org) package manager
- **Conference commitments:** IPAC19, Cyc2019 accepted investigation requests
- **Potential benefit:** Possible elimination of cloning requirements

---

## Areas Requiring Further Development

### Infrastructure Tools

| Tool Category | Current Tool | Alternative Under Investigation |
|---------------|--------------|--------------------------------|
| **Package Management** | Manual installation | [Chocolatey](https://chocolatey.org) |
| **Backup Solution** | [SyncBack Free](https://www.2brightsparks.com/syncback/syncback-hub.html) or similar | [BackupPC](https://backuppc.github.io/backuppc/) |

### System Services
- **DNS/DHCP configuration** for proceedings office
- **Status board** pre-configuration
- **Network infrastructure** optimization

### Software Licensing Strategy

| Software | Proposed Approach |
|----------|-------------------|
| **MS Office** | Trial mode utilization |
| **Windows 10** | Trial mode utilization |
| **Adobe Acrobat** | Trial mode utilization |

---

## Operational Areas for Improvement

### Conference Spaces

#### Speaker Preparation Office
- **Status:** Needs systematic approach development
- **Priority:** High - critical for conference operations

#### Paper Cafes
- **Status:** Easier to implement
- **Approach:** More straightforward setup requirements

---

## Knowledge Transfer and Documentation

### Continuous Improvement Framework

**Knowledge Sharing Paradigm:**
- Continue with established knowledge transfer practices
- Systematic documentation of lessons learned
- Regular updates to best practices

### Documentation Responsibilities

| Role | Responsibility |
|------|----------------|
| **TM IT Presenter** | Maintain and consolidate IT infrastructure documentation |
| **IPAC IT Manager** | Update wiki documentation for each conference |
| **Working Group** | Provide user feedback and test cases |

### Quality Assurance

#### User Test Cases
**Example validation process:**
- **Test scenario:** PDF MediaBox crop and "yellow dot" printing
- **Success criteria:** Expected output matches requirements
- **Failure response:** Identify and correct setup issues

**Purpose:** Validate conference IT setup before operational use

---

## Working Group Activities

### Regular Meetings
- **Participants:** Both IT experts and newcomers
- **Format:** Experience sharing and problem-solving sessions
- **Outcomes:** Best practice documentation and process improvements

### Investigation Projects
- **Chocolatey deployment** for automated software installation
- **BackupPC evaluation** for improved backup solutions
- **Trial license strategies** for commercial software

### Future Directions
- **Modernization** of traditional IT setup approaches
- **Automation** of repetitive setup tasks
- **Standardization** of conference IT procedures

---

## Key Takeaways

1. **Evolution in progress:** Moving from traditional cloning to modern package management
2. **Community-driven:** Collaborative approach to problem-solving
3. **Documentation-focused:** Systematic knowledge capture and transfer
4. **Quality-oriented:** User testing validates setup effectiveness
5. **Future-thinking:** Investigating sustainable, scalable solutions

---

## Related Resources

- [Chocolatey Package Manager](https://chocolatey.org) - Modern Windows package management
- [BackupPC](https://backuppc.github.io/backuppc/) - Enterprise backup solution
- [SyncBack Free](https://www.2brightsparks.com/syncback/syncback-hub.html) - Current backup tool option

---
