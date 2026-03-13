# Ansible Role: Bootstrap 

An Ansible Role that configure Ubuntu servers:

- Updates and upgrades packages
- Sets timezone

## Requirements

None.

Available variables are listed below, along with default values (see `defaults/main.yml`):

```yaml
# Packages
update_cache: true
upgrade_packages: true
autoremove: true
autoclean: true
cache_valid_time: 3600

# Timezone
timezone: "Europe/Kyiv"

# Example Playbook

```yaml
- hosts: all
  become: true
  roles:
    - bootstrap

# License

MIT / BSD