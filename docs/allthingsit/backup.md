# Backup System

While your editors are working at the conference venue you want to do regular backups (e.g. every evening) of their work in case a workstation fails.

For small conferences you can use a windows share on one of your machines and backup the other data to it. Windows shares are usually limit to 15 connections (if it is not enterprise windows) so this only works if you have fewer than 15 workstations.

For conferences with more workstations you should think about a dedicated system (e.g. a NAS or one computer with FreeNAS on it) to backup the data on a daily basis. 


## Backup Solutions

**FreeNAS**

URL: http://www.freenas.org/

Application:

* Dedicated backup systems for large conferences
* Network-attached storage solutions
* Daily backup scheduling
* Data redundancy and protection

Conference Implementation:

* Replace Windows share limitations (15 connections)
* Centralized backup for 15+ workstations
* Professional-grade data protection

**SyncBack Free**

https://www.2brightsparks.com/syncback/syncback-hub.html

Conference Implementation:

* Backup software that can be used to
    * collect the data from the PCs and write it to backup disk
    * installed on the PCs and backup to a e.g. windows share

**BackupPC**

https://backuppc.github.io/backuppc/

An alternative to SyncBack Free.