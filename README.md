# LTELink

> [!IMPORTANT]
> This project is a work in progress

LTELink is custom base board design for the Raxda CM3. It main purpose is to connect several IP cameras and other ethernet-connected devices on a drone, and stream their video and telemetry over LTE to a ground station.

## Hardware Specs

* 1x MiniPCIE slot for LTE modem (Designed for Quectel EC25)
* 1x Nano SIM card slot
* 1x USB 2.0 hosts
* 1x USB OTG interface with manual host/device control
* 4x 100M ethernet (unmanaged)
* 1x Micro SD card slot
* 2x UART connectors

## Hardware Block Diagram

<img width="500" alt="LTELink" src="https://github.com/user-attachments/assets/278e99bf-065a-4c06-ab64-de7e6ceed0a9" />

## Software Stack

* GStreamer for video streaming
* mavp2p for Mavlink routing
* Tailscale for VPN
* Rockchip Media Processing Pipeline for video encoding (if needed)
