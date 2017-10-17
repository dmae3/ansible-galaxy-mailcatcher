Role of installing Mailcatcher
=========

Mailcatcher ansible galaxy role.

Requirements
------------

None

Role Variables
--------------

* mailcatcher_postfix_disabled  
disable postfix

* mailcatcher_smtp_port  
Mailcatcher smtp port

* mailcatcher_http_ip  
Mailcatcher ip

* mailcatcher_http_port  
Mailcatcher http port

Dependencies
------------

[ruby](https://github.com/dmae3/ansible-galaxy-ruby.git "ruby")

Example Playbook
----------------

```yml
---
- hosts: all
  become: true
  roles:
    - { role: galaxy-mailcatcher, mailcatcher_postfix_disabled: True, mailcatcher_smtp_port: 25, mailcatcher_http_ip: 0.0.0.0, mailcatcher_http_port: 1080 }
```

License
-------

BSD

Author Information
------------------

[Daisuke Maeda](https://github.com/dmae3 "Daisuke Maeda")
