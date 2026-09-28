# Automatic Duplex Suppression for Adhesive Media

## Strict Ban on Duplex (Double-Sided) Printing

Under no circumstances should sticker sheets be passed through an automatic duplexing unit.

### Mechanical Hazards
1. **Fuser Re-Heating:** In automatic duplexing, the sheet passes through the 200°C fuser twice. The second pass dehydrates the backing paper, inducing severe curl that causes paper jams.
2. **Peel-Off in Inverter Rollers:** Duplex reversal rollers bend paper through tight 180° loops. This acute angle peels leading label edges off the backing sheet, adhering them permanently to internal drums and transfer belts.

### CSS Software Defense
Enforce single-sided printing directly in your print stylesheet:
```css
@media print {
  @page {
    /* Suppress duplexing on supported print engines */
    margin: 0;
  }
  .sheet-page {
    page-break-after: always;
    break-after: page;
  }
}
```

