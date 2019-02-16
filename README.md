Sparky Online
It checks is your web site online and display a pop up message on your dekstop.

Copyright (C) 2019 Paweł Pijanowski

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

Dependencies:
-------------
bash
coreutils
cron
iputils-ping
wget
yad

Install:
-------------
Modify sparky-online

sudo cp sparky-online /usr/bin/

sudo chmod +x /usr/bin/sparky-online

Modify sparky-online-cron

sudo cp sparky-online-cron /etc/cron.d/

sudo chown root:root /etc/cron.d/sparky-online-cron

sudo systemctl restart cron

Uninstall:
-------------
Remove both files from the system and restart cron.
