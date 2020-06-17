# Homelab-Ansible
Since I've just gotten started with Ansible, this is a place to showcase my playbooks and other work. The hope here is to share my configs with others, and possibly get feedback and ideas from others as well.

# Playbooks
The playbooks right now are fairly simple, but they help me a ton!

* **update-server.ml** - As straightforward as it sounds. Just checks for updates, and applies them, without having to manually `apt update` and `apt upgrade -y` all of the VMs separately.
* **setup-server.yml** - Update packages, install extras (open-vm-tools, apcupsd, etc.), back up the default, and template in an apcupsd config that references pfSense for the master, back up the default .bashrc for my main user, and add color to the prompts.