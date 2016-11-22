unifi-controller
================


What is does this role do?
--------------------------

This role installs the UniFi controller software from Ubiquiti.  This software is quite difficult to manage as the Ubiquiti company has not replied on several attempts to contact a representative about adjusting the license to make a native package possible.

Caveat Emptor: mongodb currently does not support block compressors on Void Linux, to get around this, the WiredTiger components are disabled in this installation.


Meta
----

Files Managed:
  * /opt/installfiles/
  * /opt/installfiles/unifi.zip
  * /opt/UniFi/data/system.properties
  * /etc/sv/UniFi
  * /etc/sv/UniFi/run
  * /etc/iptables.d/unifi.rules
  * /var/service/UniFi

Defaults Provided:
  * unifi_version: 4.8.12

Variables Required:
  * None

Optional Variables:
  * None

Files Required:
  * None

Optional Files:
  * None

Conflicting Roles:
  * None

Depends On:
  * [network](https://github.com/void-ansible-roles/network)
