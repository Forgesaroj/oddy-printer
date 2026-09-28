# Barcode Quiet Zone Engineering Specifications

## The Essential Barcode Quiet Zone (Clear Area)

A quiet zone is the blank unprinted margin surrounding a barcode symbol on all four sides.

### Dimension Rules
- **Linear 1D Barcodes (Code 128 / EAN):**
  - Minimum Quiet Zone = **$10 \times X$** (where $X$ is the narrow bar width), or **$2.54\text{ mm}$ (0.1 in)**, whichever is greater.
- **2D QR Codes:**
  - Minimum Quiet Zone = **$4 \times \text{module size}$** on all 4 borders.

### Common Defects
- Printing text, box borders, or color strips within the quiet zone makes the barcode 100% unreadable to laser scanners, because the photodiode cannot calibrate its baseline ambient reflection.

