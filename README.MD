# Klipper Configurations for Creality K1 Printer

**Note:** Install only on the official firmware with root access!

## Uploading Instructions:
- Load these configurations through `http://x.x.x.x:4408/#/configure` or navigate to the 'Configuration' section in your printer's interface.

## Fully Working Klipper Config for K1 with KAMP v8:
- **Fixed**: (SMART_PARKING) OUT OF RANGE error.
- **Added**: TIMELAPSE FOR MOONRAKER & KLIPPER (requires adding g-code in Orca printer settings, under Machine G-code (Before Layer change G-code). It should look like this:

    ```
    ;BEFORE_LAYER_CHANGE
    ;[layer_z]
    G92 E0
    TIMELAPSE_TAKE_FRAME
    ```

## In Klipper Macros:
1. Press the calibration macros in sequence.
2. Sometimes, the console will ask to press SAVE_CONFIG — do it.

## Before Starting Calibration:
Please, ensure the bed is in perfect condition, remove filament, and make sure the hotend is empty.

## Calibration:
- **PID for the hotend (PID_HOTEND)**
- **PID for the bed (PID_BED)**
- **Input Shaper (AUTOTUNE_SHAPERS)**
- **Leveling (BED_LEVELING)**
