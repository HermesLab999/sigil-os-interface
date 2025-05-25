# Sigil-OS Interface

g

This repo manages input/output between symbolic glyph controls and harmonic field commands. Built to interface with touch-panel glyph matrices and BLE command relays.

## Key Files
- `sigilos/core_parser.js` – parses sigils to action flags
- `layout/touch_matrix.svg` – touchscreen overlay (ESP32/Nextion/RA8875)
- `config/sigilmap.yaml` – user-definable glyph→command map

## Sigil Commands
```
𓂀 → reveal()
⧁ → collapse_field()
⦿ → lock_focus()
⚚ → harmonic_trigger()
```

## Integration
Call `sigil_input()` from BLE or I²C node for cross-device modulation.

∞≡∞ Licensed // 𓂀 Protocol
