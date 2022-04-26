# Inkscape: Shapes, colours, and positioning

## Drawing shapes

Let's draw some rectangles.
As before, create a document, set a width, add a grid, and zoom in.

On the left, select the rectangle tool, and draw a rectangle!

Now use the colour buttons at the bottom of the screen to change its "Fill" colour.
You can also remove the fill by clicking the cross `X`, to the left of the colours.
Hold `Shift` and click a colour to set a "Stroke" colour.

![ink](./figures-2/rect-1.png)

Note that when you selected the rectangle tool, the toolbar near the top changed:

![ink](./figures-2/rect-2.png)

Use the `Rx` field to define a radius for the corners.
(You can set different x and y radii to get odd corners, but who needs that?)

Switch to the cursor tool if you want to resize or rotate the rectangle.
But notice that the thickness of the border changes too when you do this!
Click the rectangle twice to get the skew and rotation controls:

![ink](./figures-2/rect-3.png)

What have we done!
Although this is fun, we often want to be a bit more conservative when we resize things.
Hold `Ctrl` while resizing to maintain the original aspect ratio:

![ink](./figures-2/rect-4.png)

Holding `Ctrl` when creating a new rectangle makes it square:

![ink](./figures-2/rect-5.png)

Just below the rectangle tool, you'll find the circle tool.
By default, this makes nice ellipses, but if you hold `Ctrl` (and drag the mouse in roughly the right direction) it lets you make perfect circles.
Hold `Ctrl+Shift` to draw perfect circles _centered on the first point you clicked_.

![ink](./figures-2/circle-1.png)

As with the rectangle tool, selecting the circle tool changes the toolbar shown at the top.
You can use this to manually set the circle size (to manually set position, click the cursor tool, select the circle again, and use the new toolbar that's appeared).
You can also set circle start & end points here:

![ink](./figures-2/circle-2.png)

Use the toolbar buttons to change the way fill & stroke is applied to semi-circles:

![ink](./figures-2/circle-3.png)

## Drawing paths
LINES

### Positioning and snapping

- Move, snap to different bits
- Z-index



- Rectangles, circles, text
  - Align & distribute
  - Z-index
- Stroke & fill
  - Text should never have a stroke
  - Copy-paste a style with Ctrl-Shift-V
  - Gradients? (Careful!)
  - Line endings (arrows)
  - Cap, join, order
- Paths & curves
  - Edit path
  - "Cornering" settings
  - Path intersection for zoom plots
- Fun trick: noisy data
- Guides
