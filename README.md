Role Name
=========

Dump the inventory vars

Requirements
------------

none

Role Variables
--------------
none

Dependencies
------------

none

Example Playbook
----------------

This dumps all of the facts in to ./debugvars/hosts/{{inventory_hostname}}_ansible_variables

How to include in a playbook

    - hosts: all
      roles:
        - { role: dumpvars , tags: ["vars"] }

License
-------

BSD

Author Information
------------------
George Boobyer (iAugur) Blue-Bag Ltd

Taken from answer by https://stackoverflow.com/users/2565593/steve-midgley
to:
http://stackoverflow.com/questions/18839509/where-can-i-get-a-list-of-ansible-pre-defined-variables