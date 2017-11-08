Goaccess 1.2
=========

Web logfile analyzer for Apache2

Requirements
------------

Webserver, preferred Apache2 but Nginx will also work.

Role Variables
--------------

https://goaccess.io/

Edit the systemd-service file. Change source and target file (access.log and output html file) to your liking.

Standard is /var/log/apache2/access.log and output is /var/www/html/report/index.html so you can simply call http://HOST/report to see the dashboard.

Edit the config for time and date format and VHost if needed. 

The current standard is time: H M S, date: d b Y and no VHost.

Dependencies
------------

Ncurses.
Will be installed.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename}

License
-------

BSD

Author Information
------------------

Anon, Anon0511
