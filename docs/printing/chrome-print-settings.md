# Google Chrome & Edge Print Configuration Handbook

## Complete Chrome/Edge Print Engine Calibration

Web browsers often introduce unpredictable margins and scaling when printing HTML to physical media. Follow this standard calibration procedure to achieve pixel-perfect sticker alignment.

### 1. Mandatory Dialog Options
When opening the print dialog (`Ctrl + P` / `Cmd + P`):
- **Destination:** Select your physical laser or inkjet printer.
- **Pages:** Select "All" or specify single test sheet range.
- **Layout:** **Portrait** (all Oddy A4 sheets are oriented in standard portrait 210mm × 297mm).
- **Color:** Set to **Black and White** for pure K toner barcodes or **Color** for logos.

### 2. Crucial Advanced Settings
Click **"More settings"** to reveal low-level driver controls:
- **Paper Size:** **A4** (210 × 297 mm). Do *not* use US Letter (8.5 × 11 in) which causes a 18mm vertical shift.
- **Scale:** **Custom: 100%**. Many browsers default to "Fit to paper" or "Default", which applies a 94% shrink margin that renders all row alignment useless.
- **Margins:** Set strictly to **"None"**.
- **Options Checkboxes:**
  - ✅ **Background graphics:** MUST BE CHECKED. Without this, CSS colored backgrounds, divider lines, and borders are stripped by the browser engine.
  - ❌ **Headers and footers:** MUST BE UNCHECKED. Leaving this enabled inserts page numbers and date strings that ruin the top and bottom sticker rows.

