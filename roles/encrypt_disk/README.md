# Encrypt Disk Role

This role encrypts the second disk on the server, sets it up, and mounts it.

## Variables:
- `second_disk`: The device path for the second disk (e.g., `/dev/sdb`).
- `encrypted_disk_name`: The name used for the encrypted disk mapping (e.g., `disk2`).
- `mount_point`: The directory where the disk will be mounted (e.g., `/mnt/data`).

## Usage:
```yaml
- name: Encrypt and setup the second disk
  hosts: all
  roles:
    - encrypt_disk

