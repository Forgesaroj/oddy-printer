# UPC-A Standard Barcode Formatting for Retail Export

## Universal Product Code (UPC-A) Implementation

UPC-A is the primary retail barcode standard across North America and global export markets.

### Structure (12 Digits)
- Digit 1: Number System Character (0 = regular grocery, 3 = pharma/drugs, 5 = coupons).
- Digits 2–6: Manufacturer ID.
- Digits 7–11: Item Code.
- Digit 12: Modulo 10 Check Digit.

### Optical Layout & Guard Bars
- Left Guard Bars: `101` (tall pattern extending below barcode).
- Center Separator Bars: `01010` (divides left and right 6-digit blocks).
- Right Guard Bars: `101`.
- Human Readable Text: Displayed beneath the bars in OCR-B or monospaced font.

