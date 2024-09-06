# SchoolWatch_ML
An analysis of WLAN trace data that is used to generate an average 'daily routine' for the students of each college. 

## DHCP Log CSV Structure

This table explains the structure of the `DHCP_April_2012_devType-day-*.csv` files, which logs DHCP leases for devices connected to the network.

| Column Name | Description | Example Value |
|-------------|-------------|---------------|
| `userIP`    | The IP address assigned to the user device. | 10.131.225.138 |
| `userMAC`   | The MAC address of the user device (anonymized). | 92 |
| `APNAME`    | The name of the access point the device is connected to. | lbw144-win-lap1231-1 |
| `APMAC`     | The MAC address of the access point. | 00:16:9d:e1:51:30 |
| `startTime` | The start time of the connection in Unix timestamp format. | 1334534400 |
| `endTime`   | The end time of the connection in Unix timestamp format. | 1334534428 |
| `deviceType`| The type of device (e.g., 'f' for fixed, 'c' for mobile, etc.). | f |
| `startTimeF`| The start time of the connection in human-readable format. | 2012-04-16 00:00:00 |
| `endTimeF`  | The end time of the connection in human-readable format. | 2012-04-16 00:00:28 |
| `day`       | The day of the month when the connection occurred. | 16 |

Data covers all 30 days of April 2012:
Sunday April 1st, 2012 -> Monday April 30th, 2012.

*Data was provided by the University of Florida.
Git LFS is used to maintain most of these files in this git repository.*