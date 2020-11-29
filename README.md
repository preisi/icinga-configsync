icinga2-ConfigSync
=================

This repository contains a small ansible example for an icinga2 distributed
monitoring environment without config sync and without remote command endpoint
execution. Instead of using icinga2's "remote code execution as a service" for
performing remote checks, configuration is deployed for all hosts/zones via
ansible.

Disclaimer:
-----------

As of now, this minimal ansible playbook does not support any complex hierarchy
involving any number of satellites.

Usage:
------

For this playbook, all inventory_hostnames must consist only of FQDNs. In
addition, the variable `icinga2_master` needs to be set to the FQDN of the host
running the icinga2 master node.
