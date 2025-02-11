# homeassistant

## Add ons
### DuckDNS
### File Editor
### Mosquitto broker

## Integrations
![image](https://github.com/user-attachments/assets/19fe0d5c-1cb2-4c3e-9270-e5d79d707be7)

## Entities
### Start Sonnen Charge Automation
alias: Start Sonnen Charge Automation
description: ""
triggers:
  - at: input_datetime.sonnen_start_charge
    trigger: time
conditions: []
actions:
  - action: sonnenbatterie.set_battery_reserve
    data:
      device_id: d5e9399622a1efc53acd2221dfcc5408
      value: "{{ states('input_number.sonnen_batter_buffer') | float }}"

input_text.sonnen_start_charge
input_text.sonnen_stop_charge
input_datetime.sonnen_start_charge
script.sonnen_set_mode_manual_and_charge

## Helpers




