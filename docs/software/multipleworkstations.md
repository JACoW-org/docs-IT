# Preparing Multiple Workstations

@TODO Update or scrape?

Setting up all of this once is work enough, and for small conferences it might be feasible to do it manually for 4-6 workstations.

For bigger conferences we suggest seting up a master computer and cloning the system. If you do "disk cloning" you have several options.

    Disk cloning software like Clonezilla which writes an image of a disk on e.g. an USB drive and then recreates the drives content on another machine. Clonezilla also has the possibility to clone to several systems at once through a network connection.
    Use a dedicated device, a hard disk duplicator, that connects one source and one destination disk and the data is transfered after pushing a button. 

## Preparations

    Prerequisites
        A master workstation that is already setup
        At least one huge (64 GB) USB thumb drive per person setting up. Since restoring an image is more or less automatic, the more thumb drivese the better
        The hardware of all PCs that are cloned needs to be the same (e.g. because of pre-installed drivers) 

You generalize the master and prepare it to start in setup mode. For Windows generalizing the image with "sysprep" removes any hardware-dependent information from it, resets the activation timer, and cleans up Windows so that you can duplicate the image on other computers. (Note that during TM 2017, Johan recommended not generalizing.)

    Open Sysprep.
    In the System Cleanup Action list, select Enter System Out-of-Box Experience (OOBE).
    Select the Generalize check box. (Note that during TM 2017, Johan recommended not generalizing.)
    In the Shutdown Options list, select Shutdown.
    Click OK to run Sysprep and shut down the computer. 

![](img/it_cloning_sysprep_steps.png)
	
## Cloning

    If you want to clone with Clonezilla follow the very good clonezilla instructions:
    Save Disk Image and Restore Disk Images
    If you use disk duplicaters hookup your disks and start the process:

![](img/it_cloning_hardware.jpg)