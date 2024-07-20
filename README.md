# Raspberry Pi K3s Cluster Setup

This project provides Ansible scripts to set up a [K3s](https://k3s.io/) Kubernetes cluster on Raspberry PIs.

## Requirements

- Ansible
- Raspberry Pi devices running a Debian-based OS
- SSH access to the Raspberry Pis

## Setup

1. Clone this repository:

2. Create inventory.yml with the IP addresses of your Raspberry Pi devices.

3. Run the Ansible playbook:

```bash
ansible-playbook -i inventory.yml playbook.yml
```

## Features

- Sets up K3s on Raspberry Pi.
- Configures the first Raspberry Pi as the master node.
- Joins subsequent Raspberry Pi devices as worker nodes.

## Contributing

Feel free to submit issues or pull requests if you have suggestions or improvements.
