# EAN-13 Retail Product Barcode Checksum Algorithm

## International Article Number (EAN-13) Specification

EAN-13 is the global standard for consumer retail products at point-of-sale (POS) checkout counters.

### Digit Structure
- Digits 1–3: GS1 Prefix (e.g. 890 for India, 978 for Books/ISBN).
- Digits 4–7: Manufacturer / Company Prefix.
- Digits 8–12: Item Product Code.
- Digit 13: Modulo 10 Check Digit.

### Checksum Calculation Formula (Modulo 10)
Given the first 12 digits $d_1 d_2 d_3 \dots d_{12}$:
1. Sum digits at odd positions: $O = d_1 + d_3 + d_5 + d_7 + d_9 + d_{11}$
2. Sum digits at even positions and multiply by 3: $E = 3 \times (d_2 + d_4 + d_6 + d_8 + d_{10} + d_{12})$
3. Calculate total: $T = O + E$
4. Check digit: $C = (10 - (T \pmod{10})) \pmod{10}$

```javascript
function calculateEAN13CheckDigit(code12) {
  let sum = 0;
  for (let i = 0; i < 12; i++) {
    const digit = parseInt(code12[i], 10);
    sum += (i % 2 === 0) ? digit : digit * 3;
  }
  return (10 - (sum % 10)) % 10;
}
```

