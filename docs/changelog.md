# Changelog

## 1.2

- Fix guaranteed crash-and-reboot on official firmware when tuning to channels
  8–14: the 467 MHz FRS interstitials are outside the CC1101's supported bands,
  and tuning them tripped a `furi_check` in the SubGHz HAL
- Channel validity is now probed per-firmware at startup: unsupported channels
  are skipped by channel up/down and the scanner, and shown as "N/A" in the FRS
  list (extended-range firmwares such as Unleashed/Momentum keep all 22)

## 1.1

- Scanner reliability: wait 75 ms after each retune and require 2 consecutive
  RSSI hits above squelch before pausing — stops false pauses on tuning transients
- Honest audio note: the CC1101 mirror is a digital receive-data stream, not
  demodulated analog voice — documented the app as a channel activity/RSSI scanner
- Updated app description to match

## 1.0

- Initial release
- 22 standard FRS channels with scrollable channel list
- Channel scanner with auto-pause on signal and auto-resume
- Auto-squelch with adjustable sensitivity
- Live RSSI readout and signal-strength bars
- Subchannel (privacy-code) labels 1–38
