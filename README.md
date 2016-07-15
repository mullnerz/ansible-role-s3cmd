ansible-role-s3cmd
=========

This role installs the latest version of the S3CMD package using python PIP.

Requirements
------------

No special requirements, but note that this role requires root access, so either run it in a playbook with a global `become: yes`, or invoke the role in your playbook like:

    - hosts: servers
      roles:
        - role: ansible-role-s3cmd
          become: yes

Role Variables
--------------

Available variables are listed below, along with default values (see `defaults/main.yml`):

    s3cmd_version: latest

Dependencies
------------

None.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    # Install latest version
    - hosts: servers
      become: yes
      roles:
        - ansible-role-s3cmd

    # Install specific version
    - hosts: servers
      become: yes
      roles:
        - role: ansible-role-s3cmd
          s3cmd_version: 1.6.1

License
-------

BSD

Author Information
------------------

This role was created in 2016 by [Zoltán Müllner](http://zoltan.mullner.hu/).
