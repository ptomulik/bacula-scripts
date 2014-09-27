bacula-scripts
==============

Simple scripts that may be used on bacula clients. Currently provided are
scripts for doing LVM snapshots. Tested on Debian 7.6, lvm2. 

How to
------

Download the scripts, for example::

    cd /tmp/
    wget https://github.com/ptomulik/bacula-scripts/archive/master.zip
    unzip master.zip

Copy the content of ``scripts/`` into ``/usr/local/bin/``::

    cp /tmp/bacula-resubmit-master/scripts/* /usr/local/bin/

Based on the ``*.example`` scripts, create your own scripts (without
``.example`` suffix)::

    cp /usr/local/bin/bacu_services.example /usr/local/bin/bacu_services
    vim /usr/local/bin/bacu_services  # customize the list of services
    cp /usr/local/bin/bacu_before_backup.example /usr/local/bin/bacu_before_backup
    vim /usr/local/bin/bacu_before_backup # customize the list of LVM snapshots
    cp /usr/local/bin/bacu_after_backup.example /usr/local/bin/bacu_after_backup
    vim /usr/local/bin/bacu_before_backup # customize the list of LVM snapshots

You'll find more details in the ``*.example`` scripts.


LICENSE
-------

Copyright (c) 2014 Paweł Tomulik <ptomulik@meil.pw.edu.pl>

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE

.. <!--- vim: set expandtab tabstop=2 shiftwidth=2 syntax=rst: -->
