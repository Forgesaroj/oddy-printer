# 203 DPI vs 300 DPI Discrete Pixel Snapping

## Integer Pixel Snapping for Thermal and Laser Engines

When converting continuous vector geometry into physical print dots, anti-aliased fractional pixels cause fuzzy barcode edges.

### DPI Resolution Metrics
- **203 DPI Printers:** $1\text{ dot} = \frac{25.4\text{ mm}}{203} \approx 0.1251\text{ mm}$ (5 mils).
- **300 DPI Printers:** $1\text{ dot} = \frac{25.4\text{ mm}}{300} \approx 0.0847\text{ mm}$ (3.33 mils).
- **600 DPI Laser Printers:** $1\text{ dot} = \frac{25.4\text{ mm}}{600} \approx 0.0423\text{ mm}$ (1.66 mils).

### The Snapping Rule
Bar widths must always be integer multiples of the device dot pitch ($1\times, 2\times, 3\times, \dots$). Never print a 1.5-dot bar.

