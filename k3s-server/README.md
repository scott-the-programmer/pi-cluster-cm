
Role Name
=========

k3s-setup

Description
-----------

This Ansible role is designed to install and configure a k3s server on Raspberry Pi nodes.

Requirements
------------

- SSH and network access already set up on the Raspberry Pi.
- Remote user with sudo privileges.
- Docker installed if running Molecule tests.

Role Variables
--------------

- `ansible_host`: IP Address of the Raspberry Pi node.
- `ansible_user`: SSH user for the Raspberry Pi.
- `ansible_sudo_pass`: Sudo password for the Raspberry Pi.

These variables are expected to be provided as environment variables or via the Ansible inventory.

Example Playbook
----------------

Here's an example of how to use the `k3s-setup` role:

```yaml
- hosts: raspberrypi
  roles:
    - k3s-server
```

Note: Ensure the required environment variables or inventory settings are in place when running this playbook.
