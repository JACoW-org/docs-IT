# Software Tools and Requirements, Setup, and Installation Options

![header](./img/JACoW.png "header logo")


*Contributors: Todd Satogata (Jefferson Lab)*  
*Page contact: Raphael Mueller (GSI Helmholtzzentrum für Schwerionenforschung GmbH)*  
*Last update: 2017*

---

No matter if you are running an IPAC or one of the smaller conference series, good IT support and operating workstations are key to enabling editors, presentation managers, and author reception staff to complete their activities. This talk gives details of the current software and setups required, and gives options for various conference sizes.

**Caveat:** Also see the notes from the [IT Setup Working Group](./jacow-it-setup-working-group.md) for progressive thoughts on this topic, e.g. on package management with [Chocolatey](https://chocolatey.org) and moving to Windows 10.

---

## Software Requirements by Context

Software requirements depend on the use context:

| Context | Description |
|---------|-------------|
| **Browsing / Reading** | Checking emails, signing up for things online, viewing documents |
| **Forms / Printing** | Working with forms, payments, etc. |
| **Paper and Presentation Authoring** | Work on papers and presentations as an author |
| **Paper and Presentation Processing** | Work on papers and presentations as an editor |

## Context by Location

### Primary Usage Areas

| Context | Locations |
|---------|-----------|
| **Browsing / Reading** | Internet Cafe, Dot Board, Satellite Meetings |
| **Forms / Printing** | Registration, Author Reception |
| **Paper and Presentation Authoring** | Business Office / Paper Cafe |
| **Paper and Presentation Processing** | Proceedings Office, Presentation Management / Speaker Preparation, Compatible with Auditorium(s) |

## Setup Strategy Recommendations

You could setup different contexts with different software sets, but this adds considerable configuration work.

**Recommended approach:** Use two main setups rather than multiple configurations:

1. **"Maximum" Setup (Paper and Presentation Processing)**
   - Contains everything needed
   - Use where team members are actively "working"

2. **"Minimum" Setup (Browsing / Reading)**
   - Kiosk-like environment
   - Add software individually on-site where necessary (e.g., LaTeX and Word for authors)

## Software by Context

### Browsing / Reading
- **Browsers:** Firefox, Chrome, Opera
- **Document Viewers:** PDF, DOCX, XLSX, ODT, ODS
- **Utilities:** Compression/ZIP Tool (7-Zip, WinRAR, WinZip)
- **Security:** Anti-Virus / Anti-Malware software

### Forms / Printing
*Includes all "Browsing / Reading" software plus:*

- **Typesetting/Authoring:**
  - Microsoft Word
  - LibreOffice Writer
- **PDF Tools:** PDF Creator (pdfforge PDF Creator, FreePDF)

### Paper and Presentation Authoring  
*Includes all "Forms / Printing" software plus:*

| Category | Software Options |
|----------|------------------|
| **Additional Typesetting** | Pages (macOS) |
| **TeX Environment** | MiKTeX, TeXStudio/Texmaker/TeXnicCenter |
| **PostScript Tools** | GhostView / GhostScript |
| **Presentation Software** | Microsoft PowerPoint, LibreOffice Impress, Keynote (macOS) |
| **Text Editors** | Notepad++, gvim, WinEdt |
| **Image Editing** | GIMP, Paint.NET |
| **Media Tools** | VLC Media Player, VirtualDub, K-Lite Codec Pack |

### Paper and Presentation Processing
*Includes all "Paper and Presentation Authoring" software plus:*

| Category | Software | Notes |
|----------|----------|-------|
| **PDF Processing** | Enfocus PitStop | Use trial license |
| **PDF Professional** | Adobe Acrobat Pro | Conference manages licensing |
| **Printing** | PostScript Printer Driver | Required for proper PS support |
| **Video Processing** | Handbrake, Microsoft Movie Maker, mencoder, VirtualDub | Transcoding tools |
| **Specialized Tools** | PPspliT (Transparency Splitting) | |
| **Screen Recording** | Icecreamapps Screen-Recorder | |

---

## Software Installation Process

### Installation Sequence
1. **Install Microsoft Office**
2. **Install all Windows Updates** (including Office updates)
3. **Install missing drivers** (especially graphics card)
4. **Configure PostScript printer drivers**
   - PS enabled printers are not sufficient
   - Printer driver must support PS
   - Use manufacturer's PS driver (not PCL)
5. **Install additional software** from [Recommended Software List](./jacow-recommended-software.md)

### Installation Tools
**Recommended:** [Ninite](https://ninite.com/) - Excellent for batch installation and covers most required software.

---

## Critical Software Settings

### Adobe Acrobat Print Settings
- **Page Scaling:** None
- **Auto-Rotate and center:** Yes (checked)
- **Default for PS files:** Acrobat Distiller

### Microsoft Word Configuration
- **Page scaling:** "Do not scale A4 → Letter when printing"
- **Document options:** "Save font in file" for every document when editing

### Browser Setup
- **Default homepage:** Conference SPMS instance
- **Recommended:** Use `editor.html` instead of default home page to preserve session cookies
- **Example:** `https://spms.fnal.gov/pls/tm2016/editor.html`

## PostScript Printer Driver Configuration

Access printer properties → Advanced options and set:

| Setting | Required Value |
|---------|----------------|
| **TrueType Font** | Download as Softfont |
| **PostScript Output Option** | Optimize for Portability |
| **TrueType Font Download Option** | TrueType or Native TrueType |
| **PostScript Language Level** | 2 |

![Printer Configuration](./img/printer-configuration.png "PostScript Printer Driver Configuration")

---

## Preparing Multiple Workstations

### Small Conferences (4-6 workstations)
Manual setup may be feasible for each workstation.

### Large Conferences
**Recommended:** Set up master computer and clone the system.

### Cloning Options

| Method | Description | Best For |
|--------|-------------|----------|
| **[Clonezilla](http://clonezilla.org/)** | Creates disk image on USB drive, can clone to multiple systems via network | Most conferences |
| **Hardware Duplicator** | Dedicated device for direct disk-to-disk transfer | Simple setups |

## Cloning Prerequisites

### Required Resources
- **Master workstation** (fully configured)
- **Large USB drives** (64 GB minimum, one per person setting up)
- **Identical hardware** across all PCs (for driver compatibility)

### Windows Sysprep Process

**Generalization Steps:**
1. Open Sysprep
2. **System Cleanup Action:** Enter System Out-of-Box Experience (OOBE)
3. **Generalize checkbox:** Select (Note: Johan recommended not generalizing during TM 2017)
4. **Shutdown Options:** Select Shutdown
5. Click OK to run Sysprep and shut down

![Sysprep Configuration](./img/sysprep-configuration.png "Windows Sysprep Configuration Dialog")

**Purpose:** Removes hardware-dependent information, resets activation timer, prepares for duplication.

---

## Backup System Strategy

### Small Conferences (<15 workstations)
- **Windows share** on one editor machine
- Backup other workstations to shared folder
- **Limitation:** Windows shares typically limited to 15 connections (non-enterprise)

### Large Conferences (15+ workstations)
- **Dedicated backup system** required
- **Recommendation:** [FreeNAS](http://www.freenas.org/) on dedicated computer
- **Schedule:** Daily backups (e.g., every evening)

### Backup Importance
Regular backups are essential during conference operations in case of workstation failure.

---

## Related Resources

- [IT Setup Working Group](./jacow-it-setup-working-group.md) - Progressive IT setup thoughts
- [Chocolatey](https://chocolatey.org) - Package management solutions
- [Recommended Software List](./jacow-recommended-software.md) - Complete software requirements

---
