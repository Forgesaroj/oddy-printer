# Crisp DOM Vector SVG Generation Architecture

## Direct SVG Vector Generation Architecture

Oddy Printer utilizes pure DOM vector `<svg>` generation rather than bitmap `<canvas>` blitting.

### Advantages of Native SVG
1. **Zero Blurring:** SVG elements scale infinitely without interpolation artifacts.
2. **Crisp Edge Optimization:**
```html
<svg xmlns="http://www.w3.org/2000/svg" shape-rendering="crispEdges">
  <rect x="0" y="0" width="2" height="40" fill="#000000" />
</svg>
```
`shape-rendering: crispEdges` explicitly turns off anti-aliasing filters on rectangular bars, producing razor-sharp transitions that decode instantaneously.

