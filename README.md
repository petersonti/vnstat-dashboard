### vnstat-dashboard

An adaptation of vnstat-php-frontend by bjd using Bootstrap written in PHP.

### install
`apt install vnstat`

### list network interface
`ip link show`
or
`netstat -i`

### configure
`sudo vnstat -u -i` ifaces
`sudo chown -R vnstat: /var/lib/vnstat`

### enable startup
`sudo systemctl enable vnstat
sudo systemctl restart vnstat`

### Configure VNSTAT web
$vnstat_bin_dir = <div class="text-red">'/usr/bin/vnstat'</div>;
$use_predefined_interfaces = <div class="text-red">true</div>;
if ($use_predefined_interfaces == true) {
  $interface_list = array(<div class="text-red">"eth0"</div>);
  // ...
}

### Features
* Hourly Statistics Chart (using Google Charts)
* Daily & Monthly Statistics Overview
* Top 10 Day Statistics
* Automatically populated interface selection

### Licensing
Copyright (C) 2016 Alexander Marston (alexander.marston@gmail.com)

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see <http://www.gnu.org/licenses/>.
