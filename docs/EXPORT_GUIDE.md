# Exporting & Sharing Fractals

## Export as PNG
```javascript
function exportCanvas(canvas, filename) {
    const link = document.createElement('a');
    link.download = filename || 'fractal.png';
    link.href = canvas.toDataURL('image/png');
    link.click();
}
```

## Export as SVG
Convert canvas paths to SVG for infinite resolution prints.

## High-Resolution Rendering
- Use OffscreenCanvas for 4K+ renders
- Implement tile-based rendering for memory efficiency
- Use Web Workers for background computation

## Sharing
- Generate shareable URLs with fractal parameters encoded
- Add Open Graph meta tags for social media previews
- Create animated GIFs with varying parameters
