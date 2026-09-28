# Color Profile & Barcode Contrast Optimization

## Optical Density & Color Management for Barcode Scanning

Barcode scanners do not "see" color the way the human eye does. Most warehouse and retail scanners operate using a **650nm red laser diode** or red LED array.

### The Physics of Red Laser Reflection
- **Red Ink on White Paper:** To a 650nm red laser scanner, red ink reflects red light exactly like the white background. The scanner sees pure white, making the barcode **completely invisible / unscannable**.
- **Approved Barcode Colors:** Pure Black (`#000000`), Dark Blue (`#000080`), Dark Green (`#004d00`), Dark Brown (`#3b1e08`).
- **Approved Background Colors:** White (`#ffffff`), Light Yellow (`#ffffcc`), Light Cream.

### Pure K Toner vs Composite Black
In laser printing, ensure barcodes are generated in **Pure 100% K (Black)** toner rather than 4-color CMYK Rich Black (which creates micro-registration halos and fuzzy bar edges).

