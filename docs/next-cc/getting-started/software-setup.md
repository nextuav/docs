---
sidebar_position: 4
---

# Software Setup

The NextCC Dashboard allows drone manufacturers to configure the NextCC according to their needs. Manufacturers can
check and update the tamper status of the drone, configure live stream and agriculture sensor settings, and much more,
without having to understand or work with the internals of the NextCC operating system (NextOS).

It is a simple and secure dashboard that can be opened on any web browser. Think of it as setting up your WiFi router.

This section explains how you can access the dashboard for the first time and set it up so that it becomes for you to
access it later.

## STEP 1 :

- Connect the NextCC and the Flight Controller at the TELEM port (Standard UART)
- Power up your PDB (NextCC & Flight Controller)

## STEP 2 :

- Turn on your mobile hotspot and configure it with the following detials
    - Hotspot Name – NextUAV\_EXT
    - Password – 40209357
- The NextCC is configured to automatically connect to this network [AP band = 2.4 GHz band]
- Find the IP address of NextCC using any mobile app of your preference (Download app- Network Utilities)
- Go to link: ip-of-cc:8000
- Login using the following credentials (this is configurable)
    - Username – `admin`
    - Password – `password`
