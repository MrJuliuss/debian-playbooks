## Ansible playbooks

Playbooks for debian server

## Roles

- [commons packages](roles/base)
- [git](roles/git)
- [composer](roles/composer)
- [mysql](roles/mysql)
- [nginx](roles/nginx)
- [apache](roles/apache)
- [php (for apache)](roles/php)
- [php-fpm](roles/php-fpm)
- [nodejs](roles/node)
- [ntp client](roles/ntp)
- [openvpn](roles/openvpn)
- [logwatch](roles/logwatch)
- [fail2ban](roles/fail2ban)
- [zsh](roles/zsh)

### Launch ansible : 

```
ansible-playbook playbook.yml -i hosts --user username --ask-pass --ask-sudo-pass
```

### Launch specific role in a host:

```
  ansible-playbook run_role.yml  -i 'hostname1,[hostname2, ...]' -e "ROLE={rolename}" --user {username} [--ask-pass] [--become] [--ask-become-pass]
```

Please note that at least one comma is required inside the -i arg. Example: `-i '192.168.1.10,'`
