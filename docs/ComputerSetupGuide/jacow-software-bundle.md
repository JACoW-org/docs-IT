# JACoW Software Bundle - Installation and Configuration Guide

![header](./img/header.png "header logo")
*Contributors: Raphael Mueller (GSI)*  
*Page contact: Raphael Mueller (GSI Helmholtzzentrum für Schwerionenforschung GmbH)*  
*Last update: Unknown (PDF source)*

---

*Reference: THAA03 – IT Software: Software Bundle*

This guide covers the installation and configuration of the JACoW Software Bundle for conference proceedings offices.

---

## Installation Process

### Prerequisites
- **Internet access** (preferably high-speed connection)
- **Disk space:** 5 GB minimum free space
- **Administrator privileges** required

### Installation Steps

| Step | Action | Notes |
|------|--------|-------|
| 1 | Download `JACoW_Software_Bundle.exe` | No fixed download location - contact Raphael Mueller |
| 2 | Run as Administrator | Right-click → "Run as administrator" |
| 3 | Wait for completion | Installation takes considerable time |
| 4 | Installation complete | Bundle automatically installs required software |

![Software Bundle Installation](./img/software-bundle-installation.png "JACoW Software Bundle Installation Process")

**Reference:** Wiki → for Organizers → Setting Up for the Conference → Recommended Software

---

## Post-Installation Requirements

The software bundle does **not** include everything needed. Additional manual installation required:

### Critical Manual Installations

| Component | Requirement | Notes |
|-----------|-------------|-------|
| **Microsoft Office** | Must install separately | Core productivity suite |
| **Windows Updates** | All updates including Office | Critical for security and compatibility |
| **Device Drivers** | Graphics card and other hardware | Ensure proper hardware support |
| **PostScript Printer Driver** | PS-enabled printer driver | PCL drivers insufficient - must be PostScript |

### Printer Driver Requirements
- **Not sufficient:** PS-enabled printer alone
- **Required:** PostScript printer driver from manufacturer
- **Example:** HP provides both PS and PCL drivers - use PS driver
- **Configuration:** Must configure printer driver properly

---

## Configuration Steps

### JACoW Supplemental Files
Located in "JACoW Supplemental Files" folder on Desktop:

#### Essential Configuration Files

| File | Purpose | Installation Location |
|------|---------|----------------------|
| **Acrobat9PitStop10.pdf** | Manual for Acrobat & PitStop setup | Follow instructions |
| **JACoW Media Box.eal** | PitStop configuration file | Install in PitStop |
| **SplitAnimations.ppa** | PowerPoint Plugin | PowerPoint Add-ins |

#### Installation References
- **PitStop installation:** [Enfocus PitStop Manual](http://www.enfocus.com/manuals/referenceguide/PP/11/enUS/enus/concept/c_aa1080084.html)
- **PowerPoint Add-ins:** [Office Add-ins Management Guide](http://office.microsoft.com/sq-al/access-help/view-manage-and-install-add-ins-inoffice-programs-HA010354315.aspx)

### Software-Specific Configuration

#### Adobe Acrobat
- **Printing configuration:** Page should not be "scaled to fit"
- **Default PS handler:** Distiller should be default program for PS files

#### TeXmaker Configuration
- **LaTeX distribution:** Configure to use MiKTeX
- **Integration:** Ensure proper LaTeX compilation chain

---

## Application Settings

### Microsoft Word Configuration

| Setting | Configuration | Purpose |
|---------|---------------|---------|
| **Page Scaling** | "Do not scale A4 → Letter when printing" | Maintain proper page dimensions |
| **Font Embedding** | "Save font in file" | Ensure document portability |

### Browser Setup
- **Homepage configuration:** Set to SPMS instance
- **Important:** Use `editor.html` as default page, not home page
- **Reason:** Home page clears session cookies

**Reference:** Wiki → for Organizers → Setting Up for the Conference → Software Settings

---

## Post-Cloning Considerations

After system cloning, certain configurations require re-setup:

### User-Specific Settings Lost After Cloning

| Component | Requires Reconfiguration |
|-----------|-------------------------|
| **Adobe Acrobat** | Configuration and license |
| **PitStop** | Configuration and license |
| **User preferences** | Most user-specific settings from configuration pages |

### Resolution Strategy
- **Document settings** used during initial configuration
- **Re-apply** user-specific configurations on each cloned system
- **Verify** all critical settings before conference use

---

## Troubleshooting and Support

### Common Issues
- **Long installation time:** Normal - be patient during installation
- **Missing components:** Verify all manual installation steps completed
- **Driver issues:** Ensure PostScript printer drivers properly installed
- **Configuration loss:** Expected after cloning - follow reconfiguration checklist

### Support Resources
- **Wiki documentation:** Complete configuration guides available
- **Contact:** Raphael Mueller for software bundle access and support

---

## Important Notes

**Remember:** "Questions are guaranteed in life, answers are not..."

This software bundle significantly reduces conference IT setup time but requires careful post-installation configuration for optimal performance.

---

## Related Resources

- Wiki: for Organizers → Setting Up for the Conference → Recommended Software
- Wiki: for Organizers → Setting Up for the Conference → Software Settings