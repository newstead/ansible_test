# CPU Management Role

This role disables C-states, switches CPU to performance mode, and displays CPU information.

## Usage:
```yaml
- name: Configure CPUs for performance
  hosts: all
  roles:
    - cpu_management

