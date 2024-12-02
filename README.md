# Server Preparation Playbook

This project contains an Ansible playbook and roles to prepare a server for operation.

## Roles:
1. **encrypt_disk**: Encrypts the second disk and mounts it.
2. **cpu_management**: Configures CPU settings for better performance.
3. **network_interface**: Renames the network interface to `net0`.

## Usage:

1. Install Ansible on the control machine.
2. Clone or copy this repository to your control machine.
3. Adjust the `inventory` file with the server IP addresses.
4. Configure variables like `second_disk`, `encrypted_disk_name`, and `mount_point` in the `playbook.yml`.
5. Run the playbook:

```bash
ansible-playbook -i inventory playbook.yml

