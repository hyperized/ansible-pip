hyperized.pip
=========

Simple wrapper for Python Package manager

Requirements
------------

Ansible 2.1 or above is highly recommended.

Role Variables
--------------

    pip_state: latest
    pip_executable: pip

To use pip3:

    pip_executable: pip3

Dependencies
------------

None

Example Playbook
----------------

    - hosts: all
      become: yes
      roles:
         - { role: hyperized.pip, pip_name: awscli }
         - { role: hyperized.pip, pip_name: 'requests[security]', pip_extra_args: '--upgrade' }

License
-------

MIT

Author Information
------------------

Gerben Geijteman <gerben.geijteman@fdmediagroep.nl>
