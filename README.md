Role Name
=========

Role for remounting appdir with userweb ownership

Requirements
------------

Role Variables
--------------

shared_folder

Dependencies
------------

Example Playbook
----------------

    - hosts: servers
      roles:
        - {
            role: oscbco.remount_shared_folder,
            userweb: "{{ global_user_web }}",
            shareddir: "home_{{ global_user_web }}_{{ global_appname }}",
            appdir: "/home/{{ global_user_web }}/{{ global_appname }}"
          }

License
-------

MIT

Author Information
------------------

oscbco.me
