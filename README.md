# zmk-mix

Cube studio
QQ group: 1037094476

ZMK configuration for the Mix split keyboard (nice!nano v2).

## Branches

> [!IMPORTANT]
> This repo keeps the stable ZMK `v0.3` line. Use the `zmk-v0.3` branch.

| Branch | ZMK | Description |
|---|---|---|
| [`zmk-v0.3`](../../tree/zmk-v0.3) | `v0.3` | stable ZMK v0.3 config with Cirque trackpad support and a vendored nice!view relay screen |

## External modules

Wired in via `config/west.yml`:

| Module | Revision | Purpose |
|---|---|---|
| [zmk](https://github.com/zmkfirmware/zmk) | `v0.3` | core ZMK firmware |
| [cirque-input-module](https://github.com/geeksville/cirque-input-module) | `main` | Cirque Pinnacle trackpad driver |
| [zmk-central-states-relay](https://github.com/ArtemYurov/zmk-central-states-relay) | `main` | relays state (layer, BLE, battery) from central to peripheral |

The nice!view relay screen is vendored under `boards/shields/nice_view_gem` so the peripheral display layout can be customized in this repository.
