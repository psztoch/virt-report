# virt-report
Report virtual machines using libvirt.

This tool is designed for reporting virtual machines running on multiple hosts.
However, use on a single machine can also be useful.

Please install libvirt-python. On RHEL:

    yum install libvirt-python

Then create your host list file.
Second column is not required, but shorter host name shoud be better.

You can make your host file with execution permission if you put in first line:

    #!virt-report -f

Example of use:

    myhosts -o host
    myhosts --hosts
    myhosts --guests -o mem

Abbreviations:
St - state
R - running
B - blocked
P - paused
S - during shutdown
s - shutoff
C - crashed
p - pmsuspended
A - autostart

Unit for all numbers is gigabyte (1024 * 1024 * 1024).
