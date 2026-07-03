# esphome-packages

ESPHome packages and templates for my devices.

Each device type has its own folder with a shared `package.yaml` and a matching `template.yaml` file to copy into ESPHome for a specific device.

## Using Templates

For each new device, copy the matching `template.yaml` into ESPHome, then update the values present in that template:

- `esphome.name`
- `esphome.friendly_name`
- `api.encryption.key`
- `ota.password`

For Wi-Fi devices, also update:

- `wifi.ap.ssid`
- `wifi.ap.password`

The shared `wifi_ssid` and `wifi_password` secrets can stay the same if they already exist in ESPHome.

## Bluetooth Proxy

### Files

- `bluetooth-proxy/package.yaml`
- `bluetooth-proxy/template.yaml`

### Template Values

- Replace `example-bp` with the device name.
- Replace `Example Bluetooth Proxy` with the friendly name.
- Replace the `example_bp__*` secret names with that device's secret names.
- Replace `Example-BP` with the fallback Wi-Fi AP name.

## Actron Air Serene 2

### Files

- `actron-air-serene-2/package.yaml`
- `actron-air-serene-2/template.yaml`

### Template Values

- Replace `example-ac` with the device name.
- Replace `Example AC` with the friendly name.
- Replace the `example_ac__*` secret names with that device's secret names.
- Replace `Example-AC` with the fallback Wi-Fi AP name.

## Zigbee Coordinator

### Files

- `tubezb-cc2652p7-poe-2023/package.yaml`
- `tubezb-cc2652p7-poe-2023/template.yaml`
- `tubezb-cc2652p7-poe-2023/components/stream_server/`

### Template Values

- Replace `example-zb` with the device name.
- Replace `Example Zigbee Coordinator` with the friendly name.
- Replace the `example_zb__*` secret names with that device's secret names.
- Uncomment and update `ethernet.manual_ip` if the coordinator should use a static IP.

The Zigbee coordinator package uses the vendored `stream_server` external component from this repo.

## Sonoff T1 US 3

### Files

- `sonoff-t1-us-3/package.yaml`
- `sonoff-t1-us-3/template.yaml`

### Template Values

- Replace `example-ls` with the device name.
- Replace `Example LS` with the friendly name.
- Replace the `example_ls__*` secret names with that device's secret names.
- Replace `Example-LS` with the fallback Wi-Fi AP name.
