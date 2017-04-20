dosullivan.kops
=========

This is a simple role that will install [kops](https://github.com/kubernetes/kops) for you.

Requirements
------------

This should work on pretty much any linux system.

Role Variables
--------------

There is only one variable in this role, which is the kops version to be downloaded. As of today, the most recent stable release is 1.4.4, which I've specified in defaults/main.yml like so:

    kops_version: 1.4.4

You can override this value however, as demonstrated in the example playbook below.

Example Playbook
----------------

    - hosts: servers
    - sudo: yes
      roles:
         - { role: dosullivan.kops, kops_version: 1.4.4 }

License
-------

MIT

Author Information
------------------

This role was created in 2016 by Daniel O'Sullivan.
