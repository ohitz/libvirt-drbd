libvirt-drbd
============

This script is a libvirt hook to automatically promote/demote DRBD
resources.

Place the "qemu" script in /etc/libvirt/hooks/ and it will
automatically promote and demote DRBD resources configured in libvirt
guests when the guests are started or shut down.
 
In order for the DRBD resources to be recognized as such, they need to
be configured with the /dev/drbd/by-res/<name> path.
 
The script requires the xpath command from the libxml-xpath-perl
package.

The latest version of the script is at
https://github.com/ohitz/libvirt-drbd
