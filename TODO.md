# Open Issues — Triage & TODO

Triaged 2026-06-09. Source: `gh issue list` on `atomic14/esp32-s3-pinouts`.

Legend:
- 🟢 **DOC FIX** — fixable in README/markdown text. Safe to do now.
- 🖼️ **IMAGE** — requires editing the diagram (`esp32-s3.afdesign` → `esp32-s3.webp`/`esp32-s3.pdf`). **Needs Chris to assess.**
- 🔵 **DISCUSS** — question, larger-scope feature, or unverified claim. Leave open / needs research.

---

## 🖼️ Image changes — DONE (diagram edited by Chris, committed in e9ee8ba)

- [x] **#28 — GPIO14 mislabeled `ADC1_CH3` → fixed to `ADC2_CH3`.** Factual artwork bug corrected. Issue closed.
- [x] **#36 / #14 — Diagram titled "ESP32-S3-WROOM-2".** Added a "* covers 1/1U/2" subtitle; pinout is identical across the three. #36 closed. (#14 still open for the peripheral-schematic suggestion.)
- [x] **#35 — GPIO45/46 were red "Do Not Use".** Downgraded to orange "Have default behaviours". Issue closed.

_Resolved as text-only (no diagram change):_ **#13 / #18 / #34** GPIO47/48 1.8V — closed with a dedicated README note rather than an image marker.

_No diagram change needed:_ **#22 / #26** GPIO33/34 — these are **not broken out on the WROOM-1/1U/2 modules** (no module pin), so the diagram correctly omits them. The README note explains they must be avoided in software because they map to internal Octal PSRAM/flash lines. (Issues closed.)

---

## 🟢 Doc fixes — DONE in this pass

- [x] **#32 — GPIO10 (ADC1_CH9) missing from "ADC Pins".** Added GPIO10 to the ADC1 table and added a full ADC2 table.
- [x] **#22 — Typo: GPIO34 row description says "GPIO33".** Fixed in Full GPIO Table.
- [x] **#22 / #26 — GPIO33/34 reserved for Octal PSRAM/flash.** Added note to PSRAM section.
- [x] **#13 / #18 / #34 — GPIO47/48 1.8V on "V" modules.** Added a dedicated note.
- [x] **#23 — Can GPIO43/44 (UART0) be used as output when on USB?** Yes. Added clarification.
- [x] **#16 — QIO vs DIO flash mode and GPIO9/10.** ~~Added note.~~ **Note was factually wrong (see #37) — corrected.** On the S3 the flash is on the in-package SPI0/1 bus (GPIO26–32, not broken out); GPIO9/10 are FSPI (SPI2) pins and are *always* free regardless of flash mode. The QIO/DIO reclaim trick only applies to the original ESP32. Section rewritten; #37 closed.
- [x] **#14 — Several additions:** clarified applies to WROOM-1/1U/2; 500 mA supply recommendation; weak BOOT(EN) pull-up note; GPIO-matrix 80 MHz SPI limit; "R8/R8V/V" module naming shortcut.

---

## 🔵 Discussion / research / larger scope — left open

- [ ] **#29 — Add Seeed XIAO ESP32S3 board.** Out of scope for the bare-module diagram, but repo already has DevKitC/DevKitM pages — could add a board-specific page. Needs board research.
- [ ] **#25 — Hardware SPI (IO_MUX SPI2/SPI3 pins) + MicroPython REPL.** IO_MUX default SPI pin set is worth documenting; the "avoid GPIO1/3 for REPL" claim is esp8266-sourced and dubious for S3 (REPL is over native USB-CDC). Needs verification before adding.
- [ ] **#15 — W5500 SPI only worked on certain pins.** Support question; likely IO_MUX vs GPIO-matrix ordering. Could fold into a #25 SPI note.
- [ ] **#3 — ESP32 vs ESP32-S3 register differences reference.** Useful but large, community-sourced effort. New page.
- [ ] **#2 — Which pins to isolate during sleep to cut current.** No definitive datasheet answer found (unlike ESP32 GPIO12/WROVER). Needs research.
</content>
