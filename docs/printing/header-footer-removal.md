# Complete Elimination of Browser Header & Footer Artifacts

## Eliminating Stray Browser Metadata from Sticker Sheets

By default, web browsers inject four metadata fields into printed pages:
- Top Left: Web Page Title
- Top Right: Date & Time
- Bottom Left: File Path or URL
- Bottom Right: Page Number ($X$ of $Y$)

On standard letterhead, these sit in the margins. On sticker sheets (such as ST-1, ST-40, ST-33), these print directly over your top and bottom stickers.

### Guaranteed CSS Suppression
```css
@media print {
  @page {
    margin: 0mm !important;
  }
  html, body {
    margin: 0 !important;
    padding: 0 !important;
  }
}
```
Even with CSS suppression, always uncheck **"Headers and footers"** in Chrome/Firefox print preferences.

