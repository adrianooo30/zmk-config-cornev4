# Corne wireless - ZMK config

Converted from my QMK crkbd keymap.

## Layers
0 BASE | 1 NUM/MEDIA | 2 SYM/NAV | 3 ADJUST (RGB, F-keys, Bluetooth; opens when 1+2 are held)

## Files
- `config/corne.keymap` - layers and behaviors
- `config/corne.conf`   - features (RGB underglow, OLED, sleep)
- `config/west.yml`     - ZMK version to build against
- `build.yaml`          - which boards/shields to build (nice_nano_v2 assumed)

## Use it later
1. Create an empty repo on GitHub (e.g. `zmk-config`).
2. Upload everything in this folder to it (keep `.github/` and `config/` as-is).
3. Open the Actions tab, wait for the build, download the firmware artifact.
4. Flash `settings_reset` to both halves first (double-tap reset, drag the .uf2),
   then `corne_left` and `corne_right`.
5. Remove the old Bluetooth entry on your computer and pair again.
