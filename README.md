## Ansible playbooks

Playbooks for debian server

## Roles

- [commons packages](roles/base)
- [git](roles/git)
- [composer](roles/composer)
- [mysql](roles/mysql)
- [nginx](roles/nginx)
- [php-fpm](roles/php-fpm)
- [nodejs](roles/node)
- [ntp client](roles/ntp)
- [openvpn](roles/openvpn)
- [logwatch](roles/logwatch)
- [fail2ban](roles/fail2ban)
- [zsh](roles/zsh)

### Launch ansible : 

  ansible-playbook playbook.yml -i hosts --user username --ask-pass --ask-sudo-pass

