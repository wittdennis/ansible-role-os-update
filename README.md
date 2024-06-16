# Ansible OS Update Role
Ansible role to update operating system packages

## Usage

```ansible
- name: Update OS
  roles:
    - role: wittdennis.os-update
      vars:
        os_update_reboot: "NEEDED" # possible values: NEEDED, NEVER, ALWAYS
        os_update_reboot_delay: 30
        os_update_reboot_timeout: 300
```
