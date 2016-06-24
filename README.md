# awscli

### Example
```
---

- hosts: localhost
  become: true
  vars:
    awscli_user: ubuntu
    awscli_user_home_dir: /home/ubuntu
  roles:
    - awscli
```
