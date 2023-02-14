# Lab 3 - Python

## Lesson 3 Notes

Python is a high level operating language that is unrivaled in the libraries and additional packages that are developed for the language. It is an interpreted language, generally using [CPython](https://en.wikipedia.org/wiki/CPython) to take code written Python to convert those instructions into machine code which the machine can execute. It can be installed directly from the python website or in my case, from the MSYS [python package bundler](https://packages.msys2.org/package/mingw-w64-x86_64-python).

## Lab 3 Implementation

Below is the implementation of the commands for Lab3 which utilize python and the following libraries: jdcal, astral, pytz, and geopy.

```bash

jj@jj-G3-3590:~$ cd iot
jj@jj-G3-3590:~/iot$ cd *3
jj@jj-G3-3590:~/iot/lesson3$ python3 julian.py
Calendar Date: 2023-02-13
Julian Date: 2459988.5
Modified Julian Date: 59988.0
jj@jj-G3-3590:~/iot/lesson3$ python3 date_example.py
Date: 2023-02-13
Date: 02-13-23
Day of Week: Monday
Month: February
Year: 2023
26 days after the first day of classes
80 days before the last day of classes
jj@jj-G3-3590:~/iot/lesson3$ python3 time_example.py
Mon Feb 13 23:03:23 2023
Mon Feb 13 23:03:33 2023
jj@jj-G3-3590:~/iot/lesson3$ python3 sun.py 'New York'
Information for New York/USA

Timezone: US/Eastern
Latitude: 40.72; Longitude: -74.00

Dawn:    2023-02-13 06:24:16.679789-05:00
Sunrise: 2023-02-13 06:52:59.652406-05:00
Noon:    2023-02-13 12:10:13-05:00
Sunset:  2023-02-13 17:27:57.563584-05:00
Dusk:    2023-02-13 17:56:41.814544-05:00
jj@jj-G3-3590:~/iot/lesson3$ python3 moon.py
2023-02-13 Moon Phase: 20
2023-02-14 Moon Phase: 21
2023-02-15 Moon Phase: 22
2023-02-16 Moon Phase: 23
2023-02-17 Moon Phase: 24
2023-02-18 Moon Phase: 25
2023-02-19 Moon Phase: 27
2023-02-20 Moon Phase: 0
2023-02-21 Moon Phase: 1
2023-02-22 Moon Phase: 2
2023-02-23 Moon Phase: 3
2023-02-24 Moon Phase: 4
2023-02-25 Moon Phase: 5
2023-02-26 Moon Phase: 6
2023-02-27 Moon Phase: 7
2023-02-28 Moon Phase: 8
2023-03-01 Moon Phase: 8
2023-03-02 Moon Phase: 9
2023-03-03 Moon Phase: 10
2023-03-04 Moon Phase: 11
2023-03-05 Moon Phase: 12
2023-03-06 Moon Phase: 13
2023-03-07 Moon Phase: 13
2023-03-08 Moon Phase: 14
2023-03-09 Moon Phase: 15
2023-03-10 Moon Phase: 16
2023-03-11 Moon Phase: 17
2023-03-12 Moon Phase: 18
2023-03-13 Moon Phase: 19
2023-03-14 Moon Phase: 20
jj@jj-G3-3590:~/iot/lesson3$ python3 coordinates.py 'Samuel C Williams Library'
Samuel C. Williams Library, Field House Road, Hoboken, Hudson County, New Jersey, 07030, United States
(40.74480675, -74.02532861159351)
jj@jj-G3-3590:~/iot/lesson3$ python3 address.py '40.744480675, -74.02532862031404'
Stevens Institute of Technology, Field House Road, Hoboken, Hudson County, New Jersey, 07030, United States
(40.744809599999996, -74.0252392276461)
jj@jj-G3-3590:~/iot/lesson3$ python3 cpu.py
The number of physical cores =  4
The number of logical CPUs =  8
The utilization per second as a percentage for each CPU
[0.0, 0.0, 1.0, 1.0, 2.0, 0.0, 0.0, 0.0]
[0.0, 0.0, 1.0, 0.0, 1.0, 0.0, 0.0, 0.0]
[0.0, 0.0, 2.0, 1.0, 2.0, 0.0, 0.0, 0.0]
[0.0, 2.0, 8.1, 7.1, 1.0, 7.0, 0.0, 0.0]
[3.0, 2.0, 6.0, 3.1, 3.9, 3.0, 0.0, 0.0]
[0.0, 0.0, 3.1, 10.5, 0.0, 6.0, 4.1, 0.0]
[2.0, 2.0, 4.0, 10.2, 3.0, 7.0, 1.0, 1.0]
[4.0, 0.0, 3.0, 0.0, 1.0, 4.0, 0.0, 0.0]
[1.0, 0.0, 0.0, 0.0, 2.0, 1.0, 0.0, 0.0]
[2.0, 1.0, 2.0, 0.0, 4.0, 0.0, 0.0, 0.0]
jj@jj-G3-3590:~/iot/lesson3$ python3 battery.py
sbattery(percent=83.05725079918628, secsleft=<BatteryTime.POWER_TIME_UNLIMITED: -2>, power_plugged=True)
jj@jj-G3-3590:~/iot/lesson3$ python3 documentstats.py document.txt
Word Count: 1343
Top Ten Words: [('our', 26), ('their', 20), ('has', 20), ('he', 19), ('them', 15), ('these', 13), ('have', 11), ('we', 11), ('us', 11), ('people', 10)]
```
