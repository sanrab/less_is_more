# less_is_more
Less is more ...
New navigation system (January 2023)

Router/Access Point Mango (GL-MT300N-V2)

Raspberry Zero W with RaspbianOS Lite, kplex, on-off switch (https://howchoo.com/g/mwnlytk3zmm/how-to-add-a-power-button-to-your-raspberry-pi)

Data from USB (ublox GPS, Seatalk-NMEA, dAISy, Nanobaro) to TCP port 20220

AIS data to Raymarine C-80 through USB-RS422 interface

kplex.conf

[serial]
name=ublox
filename=/dev/ttyACM0
direction=in
baud=57600
optional=yes

[serial]
name=rs422-c80
direction=out
optional=yes
filename=/dev/ttyUSB0
baud=38400
ofilter=+AI***:-all
