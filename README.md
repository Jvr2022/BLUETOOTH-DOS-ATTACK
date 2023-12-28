# Bluetooth DOS-Attack

![Logo](https://github.com/Jvr2022/BLUETOOTH-DOS-ATTACK/blob/main/src/images/logo.png)
![Python Version](https://img.shields.io/pypi/pyversions/Django.svg)

Script for conducting DOS-attacks on Bluetooth devices for pentest purposes.

## Disclaimer

This project was created for educational purposes and personal use only.

**DISCLAIMER:** This software is provided "as is" without any warranty. Usage is at your own risk. The developers assume no liability for any misuse or damage caused by this program.

## Installation

### Linux
1. Download the [Linux Release](https://github.com/Jvr2022/Bluetooth-DOS-Attack/releases).
2. Extract the release archive.
3. Open a terminal in the extracted directory.
4. Run the python script:

### Windows
1. Download the [Windows Release](https://github.com/Jvr2022/Bluetooth-DOS-Attack/releases).
2. Extract the release archive.
3. Open a terminal in the extracted directory.
4. Run the python script:

## Note

This script is designed to work only on Linux systems.You must have "l2ping" and "hcitool" utilities on your Linux machine (they are installed by default on Kali Linux).

## Tested on

- Kali Linux as the attacking platform, targeting Xiaomi Portable Bluetooth Speaker.
- Raspberry Pi W Zero as the attacker, targeting Redmi Buds Lite.

## Manual

- **Target ID or MAC:** Utilize the ID or MAC address displayed post-scanning.
- **Package Size:** Set the size of the packages to be sent to the target (600 is recommended).
- **Threads Count:** Specify the number of threads simultaneously sending packages to the target. Optimal values are provided in the table below.

|  Packages size | Threads count| Ping, ms  | Distance, meters | Time waited, sec  | Device |
|:--------------:|:-----: |:------------:|:--------------------:|:----------------:|:------:|
|  600           | 1       | 9           |0,3                   |           5      |Xiaomi Mi Portable Bluetooth Speaker|
|  600           | 10      | 38          |0,3                   |           5      |Xiaomi Mi Portable Bluetooth Speaker|
|  600           | 20      | 78          |0,3                   |           5      |Xiaomi Mi Portable Bluetooth Speaker|
|  600           | 50      | 229         |0,3                   |           5      |Xiaomi Mi Portable Bluetooth Speaker|
|  600           | 100     | 413         |0,3                   |           5      |Xiaomi Mi Portable Bluetooth Speaker|
|  600           | 200     | 806         |0,3                   |           5      |Xiaomi Mi Portable Bluetooth Speaker|
|  600           | 500     | 1961        |0,3                   |           5      |Xiaomi Mi Portable Bluetooth Speaker|
|  600           | 1000    | 6621        |0,3                   |           5      |Xiaomi Mi Portable Bluetooth Speaker|
|  600           | 1000+   | Couldn't calculate  |0,3           |           5      |Xiaomi Mi Portable Bluetooth Speaker|

## What Happens to the Target Device

While the behavior may vary between devices, the tested device typically powers off.
