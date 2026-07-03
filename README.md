# esphome-packages

ESPHome packages and templates for my devices.

Each device has a shared package file and a matching `*-template.yaml` file to copy into ESPHome for a specific device.

## Using Templates

For each new device, copy the matching `*-template.yaml` into ESPHome, then update:

- `esphome.name`
- `esphome.friendly_name`
- `api.encryption.key`
- `ota.password`
- `wifi.ap.ssid`
- `wifi.ap.password`

The shared `wifi_ssid` and `wifi_password` secrets can stay the same if they already exist in ESPHome.

## ActronAir Serene 2

### Files

- `actron-air-serene-2.yaml`
- `actron-air-serene-2-template.yaml`

### Template Values

- Replace `example-ac` with the device name.
- Replace `Example AC` with the friendly name.
- Replace the `example_ac__*` secret names with that device's secret names.
- Replace `Example-AC` with the fallback Wi-Fi AP name.

## Sonoff T1 US 3

### Files

- `sonoff-t1-us-3.yaml`
- `sonoff-t1-us-3-template.yaml`

### Template Values

- Replace `example-ls` with the device name.
- Replace `Example LS` with the friendly name.
- Replace the `example_ls__*` secret names with that device's secret names.
- Replace `Example-LS` with the fallback Wi-Fi AP name.
