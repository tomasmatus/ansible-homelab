# Homelab ansible scripts

This repository contains (will contain) various ansible playbooks that I use
to manage machines in my homelab.

## Bootstrap ansible user

Before bootsrapping set up the target in `inventory.yml`, specify the `ansib_user` and `ansible_ssh_private_key_file`.
If ssh shouldn't be used use the `--ask-pass (-k)` or `--ask-become-pass (-K)` flags to manually enter password to login
to the remote machine.

```
ansible-playbook --limit <LIMIT> bootstrap-ansible-user.yml
```

## Pi-hole update

Runs only for group `pihole`.

```
ansible-playbook playbooks/update-pihole.yml
```
