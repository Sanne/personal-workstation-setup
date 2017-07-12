## Ansible scripts for a local Fedora based Hibernate OGM developer environment

Being a Java developer needing to work on a long list of database technologies,
trying to automate my own workstation setup.
These are my own scripts, meant to setup my environment as I like it.
Feel free to check, reuse and adapt but at your own risk.

Last tested on Fedora 26 Workstation Edition

Now install Ansible; on Fedora 26 this is done by:

	sudo dnf install ansible libselinux-python python-dnf

Then run the Ansible playbook like this:

	ansible-playbook -i hosts site.yml

To run only some tagged tasks, e.g. install HipChat4 only:

  ansible-playbook -i hosts site.yml --tags "hipchat"
