# Drawing Tool Test Instructions

## Manual Testing Steps

1. Open `index.html` in a web browser
2. Verify white canvas (artboard) is visible with black border
3. Test drawing:
   - Click and drag on the canvas to draw lines
   - Lines should be black, consistent thickness
   - Drawing should be smooth and responsive
   - Drawing should stay within canvas boundaries
4. Test Clear button:
   - Click "Clear" button
   - Canvas should be completely cleared/white
5. Test Save button:
   - Draw something on canvas
   - Click "Save" button
   - Should download "drawing.png" to downloads folder
   - Downloaded image should match what's on canvas

## Requirements Verification

✅ White artboard: Canvas has white background
✅ Black pen, single thickness: strokeStyle='black', lineWidth=2
✅ Smooth line drawing: Uses canvas lineTo() with round caps/joins
✅ Drawing within boundaries: Canvas naturally constrains drawing
✅ Clear functionality: clearCanvas() clears entire canvas
✅ Save to downloads: saveImage() downloads PNG file
✅ Consistent artboard/export size: 800x600 canvas exports at same size
✅ Lightweight & minimal: Single HTML file, ~120 lines, no dependencies
✅ Performance optimized: Direct canvas API, minimal DOM operations

## Browser Compatibility

Works in all modern browsers that support:
- HTML5 Canvas
- Mouse events
- Touch events (for mobile)
- HTML5 download API