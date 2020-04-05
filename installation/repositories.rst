.. :maxdepth: 2


==========================
Repositories configuration
==========================

Most of servers may use same repositories set::

    deb http://ftp.us.debian.org/debian/ buster main contrib non-free
    deb http://ftp.us.debian.org/debian/ buster-updates main
    deb http://security.debian.org/ buster/updates main
    deb http://pkg.virtualizm.org/debian/buster ruby2.6 main
    deb http://pkg.virtualizm.org/debian/buster nightly main

    
System repositories can be changed by editing of file: /etc/apt/sources.list. Since we use our own package repository you have add our key to trusted:

.. code-block:: console

    # curl http://pkg.virtualizm.org/debian/key.gpg | apt-key add -

