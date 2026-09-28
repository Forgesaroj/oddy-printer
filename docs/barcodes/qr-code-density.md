# QR Code Matrix Density and Error Correction Levels

## Two-Dimensional QR Code Engineering Guidelines

Quick Response (QR) codes offer high information capacity and omnidirectional optical readability.

### Error Correction Levels (Reed-Solomon)
Choose the correct recovery level for your sticker environment:
- **Level L (Low):** 7% damage recovery. Smallest symbol size. Best for high-density small stickers (ST-65, ST-84).
- **Level M (Medium):** 15% damage recovery. Industrial balance (Standard for Oddy Printer).
- **Level Q (Quartile):** 25% damage recovery. Recommended for shipping labels subject to scratches and tears.
- **Level H (High):** 30% damage recovery. Allows placing corporate logos in center of code.

### Minimum Module Dimensions
To ensure instant camera decode:
- Minimum physical module size: **0.35 mm** (roughly 4 dots at 300 DPI).
- For a Version 2 code (25×25 matrix): Minimum sticker footprint is $12\text{ mm} \times 12\text{ mm}$ including quiet zone.

