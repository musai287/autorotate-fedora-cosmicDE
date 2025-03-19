# Rotate Screen Based on Orientation

A script that automatically rotates the screen based on the device's orientation using the accelerometer sensor. It is designed to work on Fedora systems with the Cosmic Desktop Environment.

## Features

- Detects the device's orientation (e.g., "normal", "right-up", "left-up").
- Rotates the screen accordingly based on the detected orientation.
- Configurable for automatic startup on user login.

## Prerequisites

- Fedora with Cosmic Desktop Environment
- `wlr-randr` for screen rotation management.
- `monitor-sensor` for monitoring device orientation.

To install the required packages:

```bash
sudo dnf install wlr-randr iio-sensor-proxy
```
