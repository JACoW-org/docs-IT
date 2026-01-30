# Preparing Multiple Workstations

Setting up all software once and configuring it is quite some work, for small conferences it might be feasible to do it manually. But for bigger conferences we suggest seting up a master computer and cloning the system.


## Setup Strategy

- **Large conferences:** Set up a "master" computer and clone other systems
- **Small conferences (4-6 PCs):** Manual setup may be more practical than having the cloning overhead


## Cloning Options

| Method | Description | Best For |
|--------|-------------|----------|
| **[Clonezilla](http://clonezilla.org/)** | Creates disk image on USB drive, can clone to multiple systems via network | Most conferences |
| **Hardware Duplicator** | Dedicated device for direct disk-to-disk transfer | Simple setups |

# Cloning Prerequisites

## Required Resources

- **Master workstation** (fully configured)
- **Large USB drives** (64 GB minimum, one per person setting up)
- **Identical hardware** across all PCs (for driver compatibility)

## Windows Sysprep Process

**Generalization Steps:**

1. Open Sysprep
2. **System Cleanup Action:** Enter System Out-of-Box Experience (OOBE)
3. **Generalize checkbox:** Select (Note: Johan recommended not generalizing during TM 2017)
4. **Shutdown Options:** Select Shutdown
5. Click OK to run Sysprep and shut down


For Windows "generalizing" the image with "sysprep" removes any hardware-dependent information from it, resets the activation timer, and cleans up Windows so that you can duplicate the image on other computers. (Note that during TM 2017, Johan recommended not generalizing.)

![](img/it_cloning_sysprep_steps.png)
	
## Cloning

If you want to clone with Clonezilla follow the very good clonezilla instructions:

[Save Disk Image and Restore Disk Images](https://clonezilla.org/clonezilla-live-doc.php)


If you use disk duplicaters hookup your disks and start the process:

![](img/it_cloning_hardware.jpg)