# Code 128 High-Density Alphanumeric Barcode Specification

## Code 128 Symbology Technical Reference

Code 128 is an ultra-high-density linear 1D barcode capable of encoding the entire 128 ASCII character set.

### Subsets
- **Code 128A:** Uppercase letters, digits, punctuation, and ASCII control characters (NUL, LF, CR, etc.).
- **Code 128B:** Uppercase and lowercase letters, digits, and standard punctuation. (Default for shipping labels).
- **Code 128C:** Double-density numeric encoding. Compresses two digits per symbol character, cutting barcode width in half. Ideal for tracking numbers and serial IDs.

### Checksum Algorithm (Modulo 103)
Code 128 includes a mandatory internal checksum character calculated as follows:
$$S = \text{Start Value} + \sum_{i=1}^{n} (\text{Value}_i \times i)$$
$$\text{Checksum Value} = S \pmod{103}$$

```javascript
function computeCode128Checksum(values, startCodeValue) {
  let sum = startCodeValue;
  for (let i = 0; i < values.length; i++) {
    sum += values[i] * (i + 1);
  }
  return sum % 103;
}
```

