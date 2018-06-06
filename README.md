# aao-pwr: Power management script for Raspberry Pi

This script allows for various functions of a Raspberry Pi to be turned off to reduce overall power consumption.

## Installation from repository

`apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 8F06D026`

`echo "deb http://apt.acousti.ca stretch main" >> /etc/apt/sources.list`

`apt-get update && apt-get install aao-pwr`

## Usage
`aao-pwr <on|off>  <usb|wifi|bluetooth|hdmi|pwrled|actled>...`

e.g.

`aao-pwr off pwrled actled`

## Compatability
The following board revisions have been tested.

|Model|Revision|Notes|
|---|---|---|
|Raspberry Pi Model B Rev 2|000d<br>000e|Power LED cannot be software controlled.|
|Raspberry Pi Model B+|0013||
|Raspberry Pi 3 Model B|a02082||
|Raspberry Pi Zero W|9000c1||
