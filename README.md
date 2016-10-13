[![Build Status](https://travis-ci.org/singleplatform-eng/ansible-role-awscli.svg?branch=master)](https://travis-ci.org/singleplatform-eng/ansible-role-awscli)

ansible-role-awscli
=========

Install and configure awscli

https://galaxy.ansible.com/singleplatform-eng/awscli/

Role Variables
--------------

- `awscli_user`: user to configure (REQUIRED)

        awscli_user: ubuntu

- `awscli_user_home_dir`: `awscli_user` home directory (REQUIRED)

        awscli_user_home_dir: "/home/{{awscli_user}}"

- `awscli_profiles`: awscli profiles to setup

        # Example
        awscli_profiles:
          - name: default
            access_key: PutYourAccessKeyHere
            secret_access_key: PutYourSecretKeyHere

Example Playbook
----------------

    ---
    - hosts: localhost
      become: true
      vars:
        awscli_user: ubuntu
        awscli_user_home_dir: /home/ubuntu
      roles:
        - awscli

Author Information
------------------

[SinglePlatform Engineering](http://engineering.singleplatform.com/)

License
-------

BSD 3-Clause
