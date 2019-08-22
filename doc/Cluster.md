# Cluster

## Setup

It is important that all timers have their clocks synchronized.
You can use NTP to do this.

### NTP

On all timers:

	sudo apt-get install ntp

On the master, edit /etc/npd.conf and add lines similar to:

	restrict 192.168.123.0 mask 255.255.255.0
	broadcast 192.168.123.255
	
On the slaves, edit /etc/npd.conf and add lines similar to:

	server 192.168.123.1

On all timers:

	sudo systemctl stop systemd-timesyncd
	sudo systemctl disable systemd-timesyncd
	sudo ​/etc/init.d/ntp restart

### Config

In config.json, under "GENERAL", add a "SLAVES" setting with
an array of IP addresses of the slave timers in track order.

```
{
	"GENERAL": {

		"SLAVES": ["192.168.1.2:5000", "192.168.1.3:5000"]

	}

}

```

Start the slave timers, then start the master.

## Notes

A slave can also be a master, but sub-splits are not propagated upwards.

If you want to use a Wi-Fi based cluster, instructions for setting up an access point (Wi-Fi hotspot) can be found at
<https://www.raspberrypi.org/documentation/configuration/wireless/access-point.md>.

