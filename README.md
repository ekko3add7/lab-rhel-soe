# lab-rhel-soe

RHEL Standard Operating Environment (SOE) automation project for Red Hat Ansible Automation Platform.

## Project overview

This project enforces a standardized RHEL 8/9 baseline via AAP Controller using Execution Environments.

## Structure

- `playbooks/` - Playbooks; `site.yml` is the master that calls all roles
- `roles/soe_*` - One role per SOE domain (base, security, users, packages, monitoring, network, compliance)
- `inventories` - Per-environment inventory and group_vars
- `execution-environment/` - EE build definition for `ansible-builder`
- `collections/requirements.yml` - Required Ansible collections
