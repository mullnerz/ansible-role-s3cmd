ansible-role-s3cmd-latest
=========

This role installs the latest version of the S3CMD package using python PIP.

Requirements
------------

No special requirements, but note that this role requires root access, so either run it in a playbook with a global `become: yes`, or invoke the role in your playbook like:

    - hosts: servers
      roles:
        - role: ansible-role-s3cmd-latest
          become: yes

Role Variables
--------------

Available variables are listed below, along with default values (see `defaults/main.yml`):

Dependencies
------------

None.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      become: yes
      roles:
         - { role: ansible-role-s3cmd-latest }

License
-------

BSD

Author Information
------------------

This role was created in 2016 by [Zoltán Müllner](http://zoltan.mullner.hu/).
