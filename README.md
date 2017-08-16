Ansible Role: Play
=========

Installs the [Play Framework](https://playframework.com/)


WIP Notice
----------

* Only installs version 1.x of the Framework
* Only tested against 1.3.x


Requirements
------------

None


Role Variables
--------------

TBD


Dependencies
------------

Any role (or other method) that will provide a compatible version of Java (6 or later). I use [this one](https://github.com/dheles/ansible-role-java).


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: all
      roles:
         - { role: play }


License
-------

CC0


Author Information
------------------

Drew Heles
