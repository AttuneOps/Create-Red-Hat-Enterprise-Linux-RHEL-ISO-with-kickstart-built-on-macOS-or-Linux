



[![Docs](https://img.shields.io/badge/docs-latest-brightgreen.svg)](http://doc.servertribe.com)
[![Discord](https://img.shields.io/discord/844971127703994369)](http://discord.servertribe.com)
[![Docs](https://img.shields.io/badge/videos-watch-brightgreen.svg)](https://www.youtube.com/@servertribe)
[![Generic badge](https://img.shields.io/badge/download-latest-brightgreen.svg)](https://www.servertribe.com/community-edition/)

# Kickstart RHEL Redhat Enterprise Linux

You might also like these projects, that integrated with physical and virtual host APIs for completely unattended building of virtual machines and physical servers:

* [Kickstart RHEL Redhat Enterprise Linux on ESXi](https://github.com/Attune-Automation/Kickstart-RHEL-Redhat-Enterprise-Linux-on-ESXi)
* Kickstart RHEL Redhat Enterprise Linux on HyperV




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

Creates a RHEL8 BIOS kickstart ISO.

### Create RHEL8 UEFI Kickstart ISO

Creates a RHEL8 UEFI kickstart ISO.

### Create RHEL9 BIOS Kickstart ISO





## Parameters


| Name | Type | Script Reference | Comment |
| ---- | ---- | ---------------- | ------- |
| Attune OS Build Server | Linux/Unix Node | `attuneosbuildserver` | This variable is used in the "Kickstart" build procedures, so the "Attune Server" can be used to build Attune servers. |
| Build Server User | Linux/Unix Credential | `buildserveruser` | The user credentials for the node building the kickstart ISO. |
| KS: Attune Base Dir | Text | `ksattunebasedir` | Base directory for deploying temporary files to build the kickstart ISO. |
| KS Linux: Disk First Letter | Text | `kslinuxdiskfirstletter` | The first letter of the disk in Linux, EG, sda or xda |
| KS Linux: Eject CDROM | Text | `kslinuxejectcdrom` | Set 1 to eject CDROM after the kickstart installation and 0 to do nothing. |
| Linux: Root User | Linux/Unix Credential | `linuxrootuser` |  |
| RHEL: 7 baseos Repo URL | Text | `rhel7baseosrepourl` | RPM Server BaseOS Repository URL for RHEL7.<br><br>For example "http://rpm_server_for_rhel7/rpm_mirror/rhel-7-server-rpms/" |
| RHEL: 8 baseos Repo URL | Text | `rhel8baseosrepourl` | RPM Server BaseOS Repository URL for RHEL8.<br><br>For example "http://rpm_server_for_rhel8/rpm_mirror/rhel-8-for-x86_64-baseos-rpms/" |
| RPM CA Certificate Drop In Directory | Text | `rpmcacertificatedropindirectory` | RPM CA Certificate drop In directory. Place all RPM CA certificates that you want to use here.<br><br>This is an absolute path to a folder. <br><br>If it does not exist or if it is empty, then it will not be used. |
| Target Server | Basic Node | `targetserver` |  |
| Target Server: Lin | Linux/Unix Node | `targetserverlin` | The target server is a generic placeholder, usually used for the server a script will run on.<br>For example, the server being built if the procedure is building a server. |
| Target Server: Linux TimeZone | Text | `targetserverlinuxtimezone` | Valid Linux timezones are listed in /usr/share/zoneinfo/posix and also at https://en.wikipedia.org/wiki/List_of_tz_database_time_zones.<br><br>Example: Australia/Brisbane |
| Target Subnet | Network IPv4 Subnet | `targetsubnet` | Subnet used by the target server. |
| RHEL: 9 baseos Repo URL | Text | `rhel9baseosrepourl` | RPM Server BaseOS Repository URL for RHEL9.<br><br>For example "http://rpm_server_for_rhel9/rpm_mirror/rhel-8-for-x86_64-baseos-rpms/" |




## Files

| Name | Type | Comment |
| ---- | ---- | ------- |
| RHEL7 BIOS Kickstart Config | Version Controlled Files | https://access.redhat.com/documentation/en-us/red_hat_enterprise_linux/5/html/installation_guide/s1-kickstart2-options |
| RHEL7 Boot ISO | Large Archives |  |
| RHEL7 grub.cfg Inside efiboot.img | Version Controlled Files | A modified "EFI/BOOT/grub.cfg" suitable for RHEL7 UEFI boot to be put in "images/efiboot.img". |
| RHEL7 UEFI Kickstart Config | Version Controlled Files |  |
| RHEL8 BIOS Kickstart Config | Version Controlled Files | RHEL8 BIOS boot files for kickstarting RHEL8. |
| RHEL8 Boot ISO | Large Archives |  |
| RHEL8 grub.cfg Inside efiboot.img | Version Controlled Files | A modified "EFI/BOOT/grub.cfg" suitable for RHEL8 UEFI boot to be put in "images/efiboot.img". |
| RHEL8 UEFI Kickstart Config | Version Controlled Files | RHEL8 UEFI boot files for kickstarting RHEL7. |
| RHEL9 Boot ISO | Large Archives | This file can be downloaded from the following link. You need a Redhat login.<br>https://developers.redhat.com/products/rhel/download#assembly-field-downloads-page-content-61451 |
| RHEL9 BIOS Kickstart Config | Version Controlled Files | RHEL9 BIOS boot files for kickstarting RHEL8. |






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
