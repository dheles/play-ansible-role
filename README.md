Ansible Role: Play 1
=========

Installs version 1.x the [Play Framework](https://playframework.com/)


Requirements
------------

None


Role Variables
--------------

    play_minimum_java_version:  1.6
    play_version_major:         1
    play_version_minor:         3
    play_version_patch:         4
    play_version:               "{{ play_version_major }}.{{ play_version_minor }}.{{ play_version_patch }}"
    play_dir:                   "play1-{{ play_version }}"
    play_download_file:         "{{ play_dir }}.tar.gz"
    play_url:                   "https://github.com/playframework/play1/archive/{{ play_version }}.tar.gz"
    play_checksum_algorithm:    "sha256"
    # NOTE: will set this dynamically, unless a value is passed in
    play_checksum:              ""
    play_download_dir:          "{{ ansible_env.HOME}}"
    play_install_dir:           "/opt"
    play_path:                  "{{ play_install_dir }}/play"


Dependencies
------------

Ansible roles (or other means) that provide the following:
  - Java 1.6 or higher
    - e.g. https://github.com/dheles/java-ansible-role
  - Python 2.5 or higher
    - Most operating systems have python pre-installed


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
