# Mathematical Analysis of Scale Distortion in Browser Engines

## The Mathematics of 100% Scaling Enforcement

When browser print engines execute the print pipeline, their default behavior is to apply a "safety margin" to prevent content clipping on consumer desktop printers. This causes catastrophic misalignment for label sheets.

### The Scale Distortion Formula
Assume an A4 sheet height of $H = 297\text{ mm}$.
If Chrome applies a default printable area margin of $0.25\text{ in}$ ($6.35\text{ mm}$) top and bottom:
$$\text{Effective Height} = 297 - (2 \times 6.35) = 284.3\text{ mm}$$
$$\text{Implicit Shrink Factor} = \frac{284.3}{297} \approx 95.72\%$$

### Compounding Alignment Error
- Row 1: Error = $0.0\text{ mm}$ (appears almost acceptable).
- Row 5: Error = $5 \times (V_p \times 0.0428) \approx 2.4\text{ mm}$ (text starts clipping label borders).
- Row 10: Error = $\approx 5.8\text{ mm}$ (completely misprinted across the die-cut line).
- Row 21 (on ST-84): Error $> 12\text{ mm}$ (entire labels print onto the wrong sticker!).

**Solution:** Always verify `transform: scale(1.0)` and browser print preview scale **100%**.

