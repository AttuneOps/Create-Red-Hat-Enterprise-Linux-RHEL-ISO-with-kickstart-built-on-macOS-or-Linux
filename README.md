



[![Docs](https://img.shields.io/badge/docs-latest-brightgreen.svg)](http://doc.servertribe.com)
[![Discord](https://img.shields.io/discord/844971127703994369)](http://discord.servertribe.com)
[![Docs](https://img.shields.io/badge/videos-watch-brightgreen.svg)](https://www.youtube.com/@servertribe)
[![Generic badge](https://img.shields.io/badge/download-latest-brightgreen.svg)](https://www.servertribe.com/community-edition/)

# Kickstart RHEL Redhat Enterprise Linux

As the demands of modern IT infrastructure grow, the need for 
efficient and standardized methods of operating system deployment 
becomes increasingly important. 

The Kickstart method is a powerful tool that allows system 
administrators to automate the installation of Red Hat Enterprise 
Linux (RHEL) on multiple machines.

This Attune Project contains Blueprints to create RHEL Kickstart ISOs.

## Understanding Kickstart Automation

Kickstart is a technology developed by Red Hat that enables 
administrators to automate the installation process of RHEL. 
Instead of manually configuring each installation, Kickstart uses a 
predefined configuration file, commonly referred to as a Kickstart 
file, to specify various installation settings. These settings 
include language preferences, partitioning schemes, package 
selection, network configuration, and more. The Kickstart file 
essentially scripts the installation process, allowing for 
consistent and repeatable deployments.

## Advantages of Automated Kickstarting

Automating the installation of RHEL using Kickstart offers several 
key benefits:

1. **Time Efficiency:** Manual installation can be time-consuming, 
especially when dealing with multiple machines. Kickstart 
automates the process, saving significant time and effort.

2. **Consistency:** Automated installations ensure that each 
instance is configured identically, reducing the risk of errors 
caused by manual intervention.

3. **Reduced Human Error:** Manual installations can lead to 
mistakes or variations in configuration. Kickstart eliminates these 
errors by following a predefined script.

4. **Standardisation:** Kickstart promotes standardized 
configurations across the organization, simplifying management and 
troubleshooting.





# Attune

[Attune](https://www.servertribe.com/)
automates and orchestrates processes to streamline deployments, scaling,
migrations, and management of your systems. The Attune platform is building a
community of sharable automated and orchestrated processes.

You can leverage the publicly available orchestrated blueprints to increase
your productivity, and accelerate the delivery of your projects. You can
open-source your own work and improve existing community orchestrated projects.

## Get Started with Attune, Download NOW!

The **Attune Community Edition** can be
[downloaded](https://www.servertribe.com/comunity-edition/)
for free from our
[ServerTribe website](https://www.servertribe.com/comunity-edition/).
You can learn more about Attune through
[ServerTribe's YouTube Channel](https://www.youtube.com/@servertribe).







# Clone this Project

To clone this project into your own instance of Attune, follow the
[Clone a GIT Project How To Instructions](https://servertribe-attune.readthedocs.io/en/latest/howto/design_workspace/clone_project.html).




## Blueprints

This Project contains the following Blueprints.



### Clean Build Files - Group

Deletes the build files and kickstart ISO group step.

### Create RHEL7 BIOS Kickstart ISO

Creates a RHEL7 kickstart ISO.

### Create RHEL7 UEFI Kickstart ISO

Creates a RHEL7 UEFI kickstart ISO.

### Create RHEL8 BIOS Kickstart ISO

Creates a RHEL8 BIOS kickstart ISO. Test

### Create RHEL8 UEFI Kickstart ISO

Creates a RHEL8 UEFI kickstart ISO.

### Create RHEL9 BIOS Kickstart ISO

Creates a RHEL9 BIOS kickstart ISO.

### Create RHEL9 UEFI Kickstart ISO


### Test RHEL Node





## Parameters


| Name | Type | Script Reference | Comment |
| ---- | ---- | ---------------- | ------- |
| IP Address for Ping Test | Text | `ipaddressforpingtest` |  |
| Kickstarted Linux Node | Linux/Unix Node | `kickstartedlinuxnode` | Refers to the node being built. |
| Kickstarted Node | Basic Node | `kickstartednode` |  |
| Kickstart Worker Linux Node | Linux/Unix Node | `kickstartworkerlinuxnode` | Linux refers to both Linux and MacOS. |
| RPM CA Certificate Drop In Directory | Text | `rpmcacertificatedropindirectory` | RPM CA Certificate drop In directory. Place all RPM CA certificates that you want to use here.<br><br>This is an absolute path to a folder. <br><br>If it does not exist or if it is empty, then it will not be used. |
| Kickstarted Node Subnet | Network IPv4 Subnet | `kickstartednodesubnet` | Subnet used by the target server. |
| Kickstart Worker Linux User | Linux/Unix Credential | `kickstartworkerlinuxuser` | The user credentials for the node building the kickstart ISO.<br>Only for Kickstart Worker Linux Node. |
| Kickstart Worker Linux User: root | Linux/Unix Credential | `kickstartworkerlinuxuserroot` | Only for Kickstart Worker Linux Node. |
| Kickstarted Linux User: root | Linux/Unix Credential | `kickstartedlinuxuserroot` | root user for "Kickstarted Linux Node". |
| Kickstarted Linux TimeZone | Text | `kickstartedlinuxtimezone` | Valid Linux timezones are listed in /usr/share/zoneinfo/posix and also at https://en.wikipedia.org/wiki/List_of_tz_database_time_zones.<br><br>Example: Australia/Brisbane |
| Kickstart Worker Base Dir | Text | `kickstartworkerbasedir` | Base directory for deploying temporary files to build the kickstart ISO. |
| RHEL8 baseos Repo URL | Text | `rhel8baseosrepourl` | RPM Server BaseOS Repository URL for RHEL8.<br><br>For example "http://rpm_server_for_rhel8/rpm_mirror/rhel-8-for-x86_64-baseos-rpms/" |
| RHEL7 baseos Repo URL | Text | `rhel7baseosrepourl` | RPM Server BaseOS Repository URL.<br><br>For example "http://rpm_server_for_rhel7/rpm_mirror/rhel-7-server-rpms/" |
| RHEL9 baseos Repo URL | Text | `rhel9baseosrepourl` | RPM Server BaseOS Repository URL for RHEL9.<br><br>For example "http://rpm_server_for_rhel9/rpm_mirror/rhel-8-for-x86_64-baseos-rpms/" |
| Kickstarted Linux Disk First Letter | Text | `kickstartedlinuxdiskfirstletter` | The first letter of the disk in Linux, EG, sda or xda |
| Kickstarted Linux Eject CDROM | Text | `kickstartedlinuxejectcdrom` | Set 1 to eject CDROM after the kickstart installation and 0 to do nothing. |
| Kickstarted Boot Loader is BIOS | Text | `kickstartedbootloaderisbios` | Set as '1' for true. |
| Kickstarted Boot Loader is UEFI | Text | `kickstartedbootloaderisuefi` | Set as '1' for true. |
| Kickstarted Operating System Name | Text | `kickstartedoperatingsystemname` | Set as:<br>"Red Hat Enterprise Linux 7",<br>"Red Hat Enterprise Linux 8", or<br>"Red Hat Enterprise Linux 9". |




## Files

| Name | Type | Comment |
| ---- | ---- | ------- |
| RHEL7 BIOS Kickstart Config | Version Controlled Files | https://access.redhat.com/documentation/en-us/red_hat_enterprise_linux/5/html/installation_guide/s1-kickstart2-options |
| RHEL7 Boot ISO | Large Archives |  |
| RHEL7 grub.cfg Inside efiboot.img | Version Controlled Files | A modified "EFI/BOOT/grub.cfg" suitable for RHEL7 UEFI boot to be put in "images/efiboot.img". |
| RHEL7 UEFI Kickstart Config | Version Controlled Files | RHEL7 UEFI boot files for kickstarting RHEL7. |
| RHEL8 BIOS Kickstart Config | Version Controlled Files | RHEL8 BIOS boot files for kickstarting RHEL8. |
| RHEL8 Boot ISO | Large Archives |  |
| RHEL8 grub.cfg Inside efiboot.img | Version Controlled Files | A modified "EFI/BOOT/grub.cfg" suitable for RHEL8 UEFI boot to be put in "images/efiboot.img". |
| RHEL8 UEFI Kickstart Config | Version Controlled Files | RHEL8 UEFI boot files for kickstarting RHEL8. |
| RHEL9 BIOS Kickstart Config | Version Controlled Files | RHEL9 BIOS boot files for kickstarting RHEL8. |
| RHEL9 Boot ISO | Large Archives | This file can be downloaded from the following link. You need a Redhat login.<br>https://developers.redhat.com/products/rhel/download#assembly-field-downloads-page-content-61451 |
| RHEL9 grub.cfg Inside efiboot.img | Version Controlled Files | A modified "EFI/BOOT/grub.cfg" suitable for RHEL9 UEFI boot to be put in "images/efiboot.img". |
| RHEL9 UEFI Kickstart Config | Version Controlled Files | RHEL9 UEFI boot files for kickstarting RHEL9. |
| Test File | Large Archives |  |






# Contribute to this Project

**The collective power of a community of talented individuals working in
concert delivers not only more ideas, but quicker development and
troubleshooting when issues arise.**

If you’d like to contribute and help improve these projects, please fork our
repository, commit your changes in Attune, push you changes, and create a
pull request.

<img src="https://www.servertribe.com/wp-content/uploads/2023/02/Attune-pull-request-01.png" alt="pull request"/>

---

Please feel free to raise any issues or questions you have.

<img src="https://www.servertribe.com/wp-content/uploads/2023/02/Attune-get-help-02.png" alt="create an issue"/>


---

**Thank you**
