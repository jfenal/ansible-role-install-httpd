Install httpd
=========

Install httpd and setup below.
* Reduce infomation in response
Add the line "ServerTokens Prod"
* Disable directory listing
Delete "Options Indexes"
* Disable welcome page
Delete welcome.conf

Requirements
------------

none

Role Variables
--------------

    # switch httpd service enabled/disabled
    httpd_service_enabled: yes

Dependencies
------------

none

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: tsyki.install-httpd, httpd_service_enabled: no }

License
-------

BSD

Author Information
------------------

Toshiyuki Imaizumi
