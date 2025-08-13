# Bluetooth Denial-of-Service (DoS) Attack Tool

![Logo](src/images/logo.png)

A Python-based tool for performing Bluetooth Denial-of-Service (DoS) attacks, intended strictly for penetration testing and security research.

[![Python Versions](https://img.shields.io/pypi/pyversions/Django.svg)](https://www.python.org/)

---

## Disclaimer

This tool is developed for educational and authorized testing purposes only.  
You are solely responsible for using it in a legal and ethical manner.

**Disclaimer:** The software is provided “as is,” without warranty of any kind. The authors are not liable for any misuse, damage, or consequences arising from its use.

---

## Installation

### Linux
1. [Download the latest Linux release](https://github.com/Jvr2022/Bluetooth-DOS-Attack/releases).
2. Extract the archive.
3. Open a terminal in the extracted folder.
4. Run the Python script.

---

## Requirements

Note: This script is designed primarily for Linux.  
Ensure the following utilities are installed:
- l2ping
- hcitool  
(Pre-installed on Kali Linux.)

---

## Tested On

- Kali Linux attacking Xiaomi Portable Bluetooth Speaker
- Raspberry Pi Zero W attacking Redmi Buds Lite

---

## Usage Guide

- Target ID / MAC: Use the address shown after scanning.
- Package Size: Number of bytes sent per packet (Recommended: 600).
- Thread Count: Number of concurrent threads sending packets.

### Performance Table

| Package Size | Threads | Ping (ms) | Distance (m) | Wait (s) | Device |
|--------------|---------|-----------|--------------|----------|--------|
| 600          | 1       | 9         | 0.3          | 5        | Xiaomi Mi Portable Bluetooth