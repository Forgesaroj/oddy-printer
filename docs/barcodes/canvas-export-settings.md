# High-Resolution Offscreen Canvas Rendering

## High-Resolution Raster Export Pipelines

For users exporting sticker sheets as PNG or PDF archives:

### High-DPI Scaling Factor
Standard browser canvases render at 96 DPI. To produce a crisp 300 DPI print-ready master:
$$\text{Scale Factor} = \frac{300}{96} = 3.125$$

```javascript
function createHighDPICanvas(widthMM, heightMM, dpi = 300) {
  const dpmm = dpi / 25.4;
  const canvas = document.createElement('canvas');
  canvas.width = Math.round(widthMM * dpmm);
  canvas.height = Math.round(heightMM * dpmm);
  const ctx = canvas.getContext('2d');
  ctx.imageSmoothingEnabled = false;
  return { canvas, ctx, dpmm };
}
```

