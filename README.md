



[![Docs](https://img.shields.io/badge/docs-latest-brightgreen.svg)](http://doc.servertribe.com)
[![Discord](https://img.shields.io/discord/844971127703994369)](http://discord.servertribe.com)
[![Docs](https://img.shields.io/badge/videos-watch-brightgreen.svg)](https://www.youtube.com/@servertribe)
[![Generic badge](https://img.shields.io/badge/download-latest-brightgreen.svg)](https://www.servertribe.com/community-edition/)

# Kickstart Linux






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



### Create RHEL8 Kickstart ISO

Creates a RHEL8 kickstart ISO.




## Parameters


| Name | Type | Script Reference | Comment |
| ---- | ---- | ---------------- | ------- |
| Attune OS Build Server | Linux/Unix Node | `attuneosbuildserver` | This variable is used in the "Kickstart" build procedures, so the "Attune Server" can be used to build Attune servers. |
| Linux: Attune User | Linux/Unix Credential | `linuxattuneuser` |  |
| KS VMWare: Attune Base Dir | Text | `ksvmwareattunebasedir` |  |
| KS Linux: Disk First Letter | Text | `kslinuxdiskfirstletter` | The first letter of the disk in Linux, EG, sda or xda |
| Target Subnet | Network IPv4 Subnet | `targetsubnet` |  |
| Target Server: Lin | Linux/Unix Node | `targetserverlin` | The target server is a generic placeholder, usually used for the server a script will run on.<br>For example, the server being built if the procedure is building a server. |
| Target Server: Linux TimeZone | Text | `targetserverlinuxtimezone` |  |
| RHEL: 8 baseos Repo URL | Text | `rhel8baseosrepourl` |  |
| Linux: Root User | Linux/Unix Credential | `linuxrootuser` |  |
| Target Server | Basic Node | `targetserver` |  |




## Files

| Name | Type | Comment |
| ---- | ---- | ------- |
| RHEL8.8 Boot ISO | Large Archives |  |
| RHEL8.7 Kickstart Config | Version Controlled Files |  |






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
