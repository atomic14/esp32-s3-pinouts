# Open Issues — Triage & TODO

Triaged 2026-06-09. Source: `gh issue list` on `atomic14/esp32-s3-pinouts`.

Legend:
- 🟢 **DOC FIX** — fixable in README/markdown text. Safe to do now.
- 🖼️ **IMAGE** — requires editing the diagram (`esp32.afdesign` → `esp32.webp`/`esp32.pdf`). **Needs Chris to assess.**
- 🔵 **DISCUSS** — question, larger-scope feature, or unverified claim. Leave open / needs research.

---

## 🖼️ Image changes — FLAGGED FOR ASSESSMENT

These can't be done from text alone; they need the Affinity Designer source edited.

- [ ] **#28 — GPIO14 mislabeled `ADC1_CH3`, should be `ADC2_CH3`.** ✅ **Confirmed bug.** The diagram labels GPIO14 as `ADC1_CH3`, which both collides with GPIO4 (the real ADC1_CH3) and contradicts the datasheet. README table is already correct. **High priority — this is a factual error in the artwork.**
- [ ] **#36 / #14 / #33 — Diagram titled "ESP32-S3-WROOM-2".** Most users have WROOM-1/1U; pinout is identical across 1/1U/2. Consider retitling to "WROOM-1/1U/2" or adding a note on the image. (Text note added to README; image still says WROOM-2.)
- [ ] **#35 — GPIO45/46 shown as red "Do Not Use".** Reporter argues they're usable with caution (inputs/outputs after boot, mind pull-down + VDD_SPI/ROM-msg roles). Decision call: keep "Do Not Use" or downgrade to "Have default behaviours / caution".
- [ ] **#13 / #18 / #34 — GPIO47/48 are 1.8V on "V" modules (R8V/R16V/R16).** Diagram shows them green "No issues". Consider a 1.8V caution marker/note for VDD_SPI=1.8V modules. (Text note added to README.)
- [ ] **#22 / #26 — GPIO33/34 not on the diagram at all.** They exist on the WROOM-2 module, are reserved for Octal PSRAM/flash, and can crash if probed. Consider adding them (with Octal-PSRAM caution styling).

---

## 🟢 Doc fixes — DONE in this pass

- [x] **#32 — GPIO10 (ADC1_CH9) missing from "ADC Pins".** Added GPIO10 to the ADC1 table and added a full ADC2 table.
- [x] **#22 — Typo: GPIO34 row description says "GPIO33".** Fixed in Full GPIO Table.
- [x] **#22 / #26 — GPIO33/34 reserved for Octal PSRAM/flash.** Added note to PSRAM section.
- [x] **#13 / #18 / #34 — GPIO47/48 1.8V on "V" modules.** Added a dedicated note.
- [x] **#23 — Can GPIO43/44 (UART0) be used as output when on USB?** Yes. Added clarification.
- [x] **#16 — QIO vs DIO flash mode and GPIO9/10.** Added note.
- [x] **#14 — Several additions:** clarified applies to WROOM-1/1U/2; 500 mA supply recommendation; weak BOOT(EN) pull-up note; GPIO-matrix 80 MHz SPI limit; "R8/R8V/V" module naming shortcut.

---

## 🔵 Discussion / research / larger scope — left open

- [ ] **#29 — Add Seeed XIAO ESP32S3 board.** Out of scope for the bare-module diagram, but repo already has DevKitC/DevKitM pages — could add a board-specific page. Needs board research.
- [ ] **#25 — Hardware SPI (IO_MUX SPI2/SPI3 pins) + MicroPython REPL.** IO_MUX default SPI pin set is worth documenting; the "avoid GPIO1/3 for REPL" claim is esp8266-sourced and dubious for S3 (REPL is over native USB-CDC). Needs verification before adding.
- [ ] **#15 — W5500 SPI only worked on certain pins.** Support question; likely IO_MUX vs GPIO-matrix ordering. Could fold into a #25 SPI note.
- [ ] **#3 — ESP32 vs ESP32-S3 register differences reference.** Useful but large, community-sourced effort. New page.
- [ ] **#2 — Which pins to isolate during sleep to cut current.** No definitive datasheet answer found (unlike ESP32 GPIO12/WROVER). Needs research.
</content>
