# Physical Hardware Margin Calibration & Digital Caliper Method

## Precision Hardware Calibration Procedure

Every printer has physical manufacturing tolerances in its feed rollers (typically ±0.5mm to ±1.5mm offset). Use this systematic methodology to eliminate physical alignment drift.

### Step 1: The Test Grid Print
1. Load a blank sheet of plain A4 copy paper (not expensive sticker sheets).
2. Generate a test sheet using your chosen Oddy SKU with border outlines enabled.
3. Print using standard 100% scale and Zero margins.

### Step 2: Caliper Measurement
Hold the printed test sheet directly over an unprinted Oddy sticker backing sheet against a strong backlit window or light table:
- **Measure Horizontal Shift ($\Delta X$):** Check if printed boxes drift left or right relative to physical die-cut lines.
- **Measure Vertical Shift ($\Delta Y$):** Check if printed boxes drift up or down.

### Step 3: Software Offset Compensation
In the Oddy Printer application, adjust the millimetric shift sliders:
```css
:root {
  --calibration-offset-x: +0.75mm; /* Positive moves content right, negative moves left */
  --calibration-offset-y: -1.20mm; /* Positive moves content down, negative moves up */
}
```
Re-verify with a second plain paper print before running live production sticker sheets.

