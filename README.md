# LibreNMS-Agent-SELinux
LibreNMS Agent SELinux Modules.

These are created for CentOS7/CentOS8 and LibreNMS Agent running with SNMP. Use at your own risk.

## Apache
Use the module in this repo.
Expects the temp file to be written to /tmp and not /var/cache/librenms

## ISC DHCP
Use the module in this repo.

## Bind/Named
Use the module and also set this sebool
```setsebool -P nis_enabled 1```

## ZFS
Use the module in this repo.
This policy allows snmpd_t to ioctl, open, read and write against device_t. This is a potentially dangerous policy, use at your own risk!

## About

This reposistory is full of SELinux Modules for LibreNMS-Agent while maintaining a Cluster (UKI-SCOTGRID-DURHAM) for [GridPP](https://www.gridpp.ac.uk/) when I was working at the [IPPP](https://www.ippp.dur.ac.uk) part of [Durham University](https://www.dur.ac.uk).

More from me at my [website](http://www.aboutcher.co.uk).
