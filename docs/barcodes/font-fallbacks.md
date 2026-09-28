# Cross-Platform Monospaced Typography Stacks

## Robust Typography Systems for Label Printing

Sticker printing requires exact font metric predictability across Windows, macOS, Android, and Linux.

### Recommended CSS Stacks
```css
/* Monospaced stack for SKU and Price formatting */
.price-tag {
  font-family: ui-monospace, 'SF Mono', 'Cascadia Code', 'Segoe UI Mono', 
               'Liberation Mono', Menlo, Monaco, Consolas, monospace;
  font-feature-settings: 'tnum' 1, 'zero' 1;
}

/* High-contrast sans stack for product titles */
.sticker-title {
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, 
               'Helvetica Neue', Arial, sans-serif;
  font-weight: 700;
  letter-spacing: -0.01em;
}
```
`tnum` enables tabular proportional numbers so decimal places in price tags align perfectly vertically.

