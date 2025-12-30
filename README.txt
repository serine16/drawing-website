Basic Setup:
    - Created an HTML5 page with a centered layout
    - Added a canvas to draw on
    - Added base JavaScript to handle mouse events (mousedown, mouseup, mousemove)

Drawing Logic:
    - Used ctx.lineTo() + ctx.stroke() for smoother pen lines
    - Stored mouse position with lastX, lastY for clean strokes

Brush Customization:
    - Added a Brush Size Slider using input type="range"
    - Added a Color Picker using input type="color"
    - Added a Brush Style Selector (pen, spray, square) with select

Undo and Redo System:
    - Created undoStack and redoStack to store drawing history
    - Used canvas.toDataURL() to save and restore canvas snapshots
    - Bound keyboard shortcuts:
        Ctrl + Z → Undo
        Ctrl + U → Redo

Saving as PNG:
    - Added a “Save PNG” button
    - Used canvas.toDataURL() + anchor click to download the drawing as an image

