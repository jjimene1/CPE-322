# Lab 5 Paho-MQTT

## Lesson 5 Notes

Paho-MQTT is a code base that provide a client class which enables applications to connect to an MQTT broker to publish messages, and to subscribe to topics and receive published messages. It also provides some helper functions to make publishing one off messages to an MQTT server very straightforward. The MQTT protocol is a machine-to-machine (M2M)/”Internet of Things” connectivity protocol. Designed as an extremely lightweight publish/subscribe messaging transport, it is useful for connections with remote locations where a small code footprint is required and/or network bandwidth is at a premium.

## Lab 5 Implementation

For working on my local Windows Machine I had to install Paho-MQTT using the MSYS installation environment. The installation command can be found in the following [link](https://packages.msys2.org/package/mingw-w64-clang-x86_64-paho.mqtt.c?repo=clang64). Following the installation for Paho-MQTT, the following commands were used to implement lab 5.

```bash
cd iot 
git pull
cd lesson5
python3 subcpu.py
```

This will activate the subscriber and will wait for the publisher to send a message. In a separate terminal window, the following commands were used to publish a message to the broker.

```bash
cd iot 
git pull
cd lesson5
python3 pubcpu.py
```

The following is the output from the subscriber terminal window.

```bash
Juan Jimenez@DESKTOP-JQOE2UL MINGW64 ~/iot/lesson5
$ python3 subcpu.py
Connected with result code 0
MyCPU 2023-03-04 14:46:44
MyCPU CPU Usage:   22.1 %
MyCPU 2023-03-04 14:46:54
MyCPU CPU Usage:   9.8 %
MyCPU 2023-03-04 14:47:04
MyCPU CPU Usage:   11.9 %
MyCPU 2023-03-04 14:47:14
MyCPU CPU Usage:   14.0 %
```

## Eclipse Mosquitto and Eclipse Paho

### Install on Rapsberry Pi

```bash
jjimenez@raspberrypi:~ $ sudo apt-get install mosquitto mosquitto-clients
jjimenez@raspberrypi:~ $ mosquitto_sub -h localhost -v -t "\$SYS/#"
```

### On Raspberry Pi OS (Bullseye), change /opt/vc/bin/vcgencmd to /usr/bin/vcgencmd in system_info.py

* Copy ~/iot/lesson5/system_info.py to ~/demo
* Copy ~/iot/lesson5/subraspi.py to ~/demo
* Copy ~/iot/lesson5/pubraspi.py to ~/demo
* Replace topic "Raspberry Pi" with a unique hostname in both subraspi.py and pubraspi.py
* Run subraspi.py on Terminal 1 and pubraspi.py on Terminal 2

This is the output on my Raspberry Pi 4B.

Subscriber:

```bash
jj Temperature: 53.0 C
jj CPU Usage:   0.2 %
jj 2023-03-07 19:18:42
jj Temperature: 53.5 C
jj CPU Usage:   0.2 %
jj 2023-03-07 19:18:52
jj Temperature: 52.5 C
jj CPU Usage:   0.2 %
jj 2023-03-07 19:19:02
jj Temperature: 53.5 C
jj CPU Usage:   0.3 %
jj 2023-03-07 19:19:12
jj Temperature: 54.0 C
jj CPU Usage:   3.2 %
jj 2023-03-07 19:19:22
jj Temperature: 53.5 C
jj CPU Usage:   2.0 %

```

Publisher:

```bash
Free RAM: 99 (3838)
Number of processes: 192
Up time: 13 days,  4:43
Number of connections: 6
Temperature in C: 53.0
IP-address: 192.168.1.179
/bin/sh: 1: /opt/vc/bin/vcgencmd: not found
CPU speed in MHz:
2023-03-07 19:14:47
```