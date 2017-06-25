ACL Updater for DynDNS
======================

## License
Script for updating NGINX and UFW ACL with a Dynamic IP Address

This is based on the work from this discussion : https://unix.stackexchange.com/questions/91701/ufw-allow-traffic-only-from-a-domain-with-dynamic-ip-address

This script is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This script is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this script.  If not, see <http://www.gnu.org/licenses/gpl.txt>

## Tested on
Debian 8 and Debian 9

## Installation

```bash
cd /root/
wget https://raw.githubusercontent.com/stylersnico/acl-updater-for-dyndns/master/dinhost.sh
chmod +x dinhost.sh
echo "1.2.3.4" > /var/log/dinhost.log
sed -i 's/'dyn.host'/'your.dydns'/g' /root/dinhost.sh
./dinhost.sh
```


