# Network Interface Role

This role renames the active network interface to `net0` and displays information about it.

## Usage:
```yaml
- name: Rename and display network interface
  hosts: all
  roles:
    - network_interface

