# Ansible-Mailserver-setup

## Requirements
- ansible2.9
- centos7
- python3

## hosts file

```
# Hosts
[MailServer]
yourmailserver-domain.com ansible_host=

# Vars
[MailServer:vars]
ansible_ssh_pass=
```

## Various conf files
Modify it according to your settings.

```
roles/postfix-setup/templates
```

## run command

```
ansible-playbook -i hosts mailserver-setup.yml
```
