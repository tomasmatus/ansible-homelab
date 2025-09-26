# Homelab ansible scripts

This repository contains (will contain) various ansible playbooks that I use
to manage machines in my homelab.

## Pi-hole update

Runs only for group `pihole`.

```
ansible-playbook playbooks/update-pihole.yml
```
