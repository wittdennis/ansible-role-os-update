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
        os_update_cleanup: true # specifies if unneeded packages and caches should be cleaned after update
        os_update_dnf_excludes: [] # List of excludes for a dnf upgrade
        os_update_dist_upgrade: true # Sets if distro should be updated also (currently only works for Debian os family)
```
