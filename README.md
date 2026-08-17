# Battery Display for LILYGO T-Display-S3

Wireless dashboard firmware for the LILYGO T-Display-S3. It displays live Battery Emulator data received over ESP-NOW or through a local Wi-Fi network.

## Web installer

Open the GitHub Pages link for this repository in Google Chrome or Microsoft Edge, connect the T-Display-S3 by USB, and choose:

- **Update firmware** to preserve the saved network, ESP-NOW, brightness, and screen settings.
- **Factory install** for a new board or complete recovery.

The installer shows the current stage, percentage, and progress bar while writing.

## First-time phone setup

When phone setup is active, the display shows:

- Wi-Fi: `BatteryDisplay-Setup`
- Password: `123456789`
- Address: `192.168.4.1`

The title changes to `PHONE CONNECTED` when a phone joins the setup network.

## Features

- Four switchable dashboard screens
- Direct ESP-NOW mode without a router
- Home Wi-Fi mode with automatic reconnection
- Phone-based first-time configuration
- Web control for brightness, start screen, theme, and SOC badge
- Preserved settings during normal firmware updates
- Cell voltage graph with minimum, maximum, cell numbers, and delta
- Connection and battery-status diagnostics

## Build from source

The project uses PlatformIO and the `lilygo-t-display-s3` environment.

```text
platformio run -e lilygo-t-display-s3
```

Source code is in `src/main.cpp`. Prebuilt firmware images used by the web installer are in `firmware/`.

## Hardware

- LILYGO T-Display-S3
- ESP32-S3
- 320 × 170 color display

## Version

Firmware 12.2 CLIENT
