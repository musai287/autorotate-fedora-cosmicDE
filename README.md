

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

## Installation

-  Clone the repository:
```bash
git clone https://github.com/your-username/rotate-screen.git
```
-  Navigate to the project folder:
```bash
cd rotate-screen
```
-  Make the script executable:
```bash
chmod +x rotate-screen.sh
```
-  (Optional) For Automatic Startup
   To have the script run automatically on startup, follow these steps:
   Move the rotate-screen.sh script to /usr/local/bin/:
```bash
sudo mv rotate-screen.sh /usr/local/bin/
```
-   Move the rotate-screen.desktop file to ~/.config/autostart/:
```bash
    mkdir -p ~/.config/autostart
    cp rotate-screen.desktop ~/.config/autostart/
```
- If the autostart folder doesn't exist in ~/.config/, you can create it manually with the mkdir command above.

## Usage

To run the script manually, execute:
```bash
./rotate-screen
```
