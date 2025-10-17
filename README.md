# Sofle

This is a fork of the [zmk-sofle](https://github.com/a741725193/zmk-sofle) project with my own keymap.

Also, It uses custom shield from [nice-view-battery](https://github.com/infely/nice-view-battery) project.

## Keymap

![Keymap](keymap-drawer/eyelash_sofle.svg)

## Building Firmware

To build the firmware, navigate to the GitHub Actions tab in this repository and manually trigger the build workflow. The workflow will generate firmware files that you can download as artifacts.

## Flashing Instructions

Follow these steps carefully to flash your Sofle keyboard:

### Step 1: Flash the Left Side

1. Enter bootloader mode on the left half (double-tap the reset button)
2. Flash with `settings_reset-eyelash_sofle_left-zmk.uf2`
3. Enter bootloader mode on the left half again
4. Flash with `eyelash_sofle_studio_left.uf2`

### Step 2: Flash the Right Side

1. Enter bootloader mode on the right half (double-tap the reset button)
2. Flash with `settings_reset-eyelash_sofle_left-zmk.uf2`
3. Enter bootloader mode on the right half again
4. Flash with `nice_view_adapter nice_view_battery-eyelash_sofle_right-zmk.uf2`

### Step 3: Reconnect Bluetooth

Since the settings were reset, you'll need to reconnect the keyboard to your device via Bluetooth.
