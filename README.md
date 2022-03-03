Simple Grafana deployment and minor adjustments to `/etc/grafana/grafana.ini`. The playbook is intended to run in the RedHat Demo environment.

## Requirements
Minimum Ansible requirements:

* ansible-core

The following Ansible Collections are necessary:

* community.general
* community.grafana

Missing collections can be installed with the provided `requirements.yml` file.
```bash
ansible-galaxy collection install -r requirements.yml
```

## Execution
Adjust the inventory file, the `main.yml` references the group *grafana*, create the group and add a host to it. 

Execute playbook (inventory is set in *ansible.cfg*):
```bash
ansible-playbook main.yml
```

## Author
Created 2022 by Tim Grützmacher
