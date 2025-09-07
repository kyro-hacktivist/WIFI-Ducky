<h1 align="center">pico-ducky</h1>

<div align="center">
  <strong>Make a easy but powerful USB Rubber Ducky with a Raspberry Pi Pico w</strong>
</div>

<br />

<div align="center">
  <img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/dbisu/pico-ducky">
  <img alt="GitHub license" src="https://img.shields.io/github/license/dbisu/pico-ducky">
  <a href="https://github.com/dbisu/pico-ducky/graphs/contributors"><img alt="GitHub contributors" src="https://img.shields.io/github/contributors/dbisu/pico-ducky"></a>
  <img alt="GitHub commit activity" src="https://img.shields.io/github/commit-activity/m/dbisu/pico-ducky">
  <img alt="GitHub Repo stars" src="https://img.shields.io/github/stars/dbisu/pico-ducky">
</div>

<br />

## Quick Start Guide
Install and have your USB Rubber Ducky working in less than 5 minutes.
1. Plug the device into a USB port while holding the boot button. It will show up as a removable media device named (`RPI-RP2`).
   Install CircutlPython on the Pico W.
   Copy the (`adafruit-circuitpython-raspberry_pi_pico_w-en_US-9.2.1.uf2`) file to the root of the Pico (`RPI-RP2`). The device will reboot and after a second or so, it will reconnect as (`CIRCUITPY`).

2. Extract and copy the lib folder to the root of the (`CIRCUITPY`).

3. Copy *.py to the root of the (`CIRCUITPY`).

4. Follow the instructions in `README.md` to enter setup mode.

5. Copy your payload as (`payload.dd`) to the root of the (`CIRCUITPY`).

6. The `WIFI AP` and `password` for the Ducky is stored in `secrets.py`, to inject / edit payloads wirelessly. 

7. Unplug the device from the USB port and remove the setup jumper.

Enjoy your Pico-Ducky.

## Setup mode

To edit the payload, enter setup mode by connecting the pin 1 (`GP0`) to pin 3 (`GND`), this will stop the pico-ducky from injecting the payload in your own machine.

The easiest way to do so is by using a jumper wire between those pins as seen bellow.

![Setup mode with a jumper](images/setup-mode.png)
