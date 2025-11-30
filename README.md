# LTELink

> [!IMPORTANT]
> This project is a work in progress

LTELink is custom base board design for the [Radxa CM3](https://radxa.com/products/cm/cm3/). It main purpose is to connect several IP cameras and other ethernet-connected devices on a drone, and stream their video and telemetry over LTE to a ground station. Additionally, a compatible WiFi adapter could be connected via USB to use [WFB-ng](https://github.com/svpcom/wfb-ng) for a direct radio link. Video streamed through the LTELink could also be recorded directly to the onboard SD card for a post-flight review.

<img width="500" src="https://github.com/user-attachments/assets/ca9d052e-c7c2-421a-a9f2-2f978cc6fd84" />

## Hardware Specs

* 1x MiniPCIE slot for LTE modem (Designed for Quectel EC25)
* 1x Nano SIM card slot
* 1x USB 2.0 hosts
* 1x USB OTG interface with manual host/device control
* 4x 100M ethernet (unmanaged)
* 1x Micro SD card slot
* 2x UART connectors

## Hardware Block Diagram

<img width="500" src="https://github.com/user-attachments/assets/699ff77e-5bd5-4a6f-891a-a9c4c4d0e533" />

## Software Stack

* GStreamer for video streaming
* mavp2p for Mavlink routing
* Tailscale for VPN
* Rockchip Media Processing Pipeline for video encoding (if needed)
