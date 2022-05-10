# Inkscape: Shapes, colors, text, and lines

## Drawing shapes

Let's draw some rectangles.
As before, create a document, set a width, add a grid, and zoom in.

On the left, select the rectangle tool, and draw a rectangle!

Now use the colour buttons at the bottom of the screen to change its "Fill" colour.
You can also remove the fill by clicking the cross `X`, to the left of the colours.
Hold `Shift` and click a colour to set a "Stroke" colour.

![ink](./figures/rect-1.png)

Note that when you selected the rectangle tool, the toolbar near the top changed:

![ink](./figures/rect-2.png)

Use the `Rx` field to define a radius for the corners.
(You can set different x and y radii to get odd corners, but who needs that?)

Switch to the cursor tool if you want to resize or rotate the rectangle.
But notice that the thickness of the border changes too when you do this!
Click the rectangle twice to get the skew and rotation controls:

![ink](./figures/rect-3.png)

What have we done!
Although this is fun, we often want to be a bit more conservative when we resize things.
Hold `Ctrl` while resizing to maintain the original aspect ratio:

![ink](./figures/rect-4.png)

Holding `Ctrl` when creating a new rectangle makes it square:

![ink](./figures/rect-5.png)

Just below the rectangle tool, you'll find the circle tool.
By default, this makes nice ellipses, but if you hold `Ctrl` (and drag the mouse in roughly the right direction) it lets you make perfect circles.
Hold `Ctrl+Shift` to draw perfect circles _centered on the first point you clicked_.

![ink](./figures/circle-1.png)

As with the rectangle tool, selecting the circle tool changes the toolbar shown at the top.
You can use this to manually set the circle size (to manually set position, click the cursor tool, select the circle again, and use the new toolbar that's appeared).
You can also set circle start & end points here:

![ink](./figures/circle-2.png)

Use the toolbar buttons to change the way fill & stroke is applied to semi-circles:

![ink](./figures/circle-3.png)

### Mirror, rotate, and flip

If you switch back to the cursor tool and select a circle, the top toolbar should also show you buttons to flip, mirror, and rotate your shape:

![ink](./figures/moving-1.png)

### Z-index

Make a few copies of your item (remember to use Ctrl+Alt+V if you want to copy the position too), and 
move them so that they overlap.
You can control which objects is shown on top with the z-index controls, indicated below:

![ink](./figures/moving-2.png)

## Drawing lines

Now let's try the line tool.
Pick a first point, and then a second, third, and so on.
Holding `Ctrl` lets you draw horizontal or vertical line segments.
To stop, do a right click anywhere on the page.

Depending on what your "Fill" and "Stroke" colours are, you should get something like these:

![ink](./figures/lines-1.png)

## Fill and stroke

Now let's play with fill and stroke in a bit more detail.
Clear the page (select items and hit `delete`, or use `Ctrl+A` to select all and hit delete just once).
Now use the line tool to draw a shape, e.g.:

![ink](./figures/fs-1.png)

Now open the `Fill and Stroke` dialog. 
You might already see it on the right of your screen, perhaps after toggling the dialogs on/off with F12.
If not, use the menu open `Objects > Fill and Stroke`.
Or if you want to feel like a pro, use `Ctrl+Shift+F` to open this dialog.

![ink](./figures/fs-2.png)

Using this dialog, you can control the fill & stroke settings of your object in detail.
For example, to set a simple "flat color" as shown above.

The first thing you'll want to do, is set the colour picking tool to either [HSL or HSV](https://en.wikipedia.org/wiki/HSL_and_HSV).
HSV is my favourite.
In this mode of colour selection, you can quite easily find good colour combinations by leaving S (saturation) and V (for _value_, or brightness) fixed at their values, and simply varying H (hue).

(For primary colours, hue=colour, but in general the human concept of "colour" is more complex than this. For example "pink" and "brown" are certain hue/brightness/saturation combinations, while things like "golden" include shinyness and reflections and whatnot. There's also [stuff](https://en.wikipedia.org/wiki/Watercolor_illusion) like [this](https://en.wikipedia.org/wiki/Checker_shadow_illusion).)

The fourth slider lets you set the "alpha" or transparency value.
This can give some nice effects, but don't get carried away: many journals only accept the `EPS` format for vector graphics, which doesn't support transparency.

At the bottom right you'll find an RGBA field where you can enter HEX codes.
This is particularly useful if you want to copy-paste colour values from other software.

Besides "flat color", you can also try using a (linear or radial) gradient.

![img](./figures/fs-3.png)

Customising gradients is fiddly.
Select the gradient in the `Fill and Stroke` dialog, then select the path editing tool top-left (just below the cursor).
Now you can change the gradient orientation, and change the colour associated with each end (which also uses the Fill & Stroke dialog, so lots of potential for confusion).

![img](./figures/fs-4.png)

A drawback of using fancier rendering options like these is that the gradient will have to be recreated by any viewer or printer that renders the file.
The more complicated the instruction, the less likely it is that the figure will always render the same.

### Customising stroke style

The `Stroke paint` panel lets you set a stroke colour the same way you did for the fill.
You can even use gradients here, to create lines that fade into nothing.
The next panel, `Stroke style` has more useful options.

First, it lets you set line widths and line styles.
Try and define widths in physical units (pt, inch, mm) rather than pixels, and use only a handful of line widths in a single figure.

If you're using a patterned line style, e.g. with dashes, you can use the `offset` controls to the right of the line style selector to tweak where the dashes fall:

![img](./figures/fs-5.png)

You can also add markers for the start, middle, and end of a line:

![img](./figures/fs-6.png)

Unfortunately, this requires you to remember which was the start and end when you drew the line.
And arrow heads don't coincide with line endings, so some tweaking is often required to get nice results.

The `join` control lets you choose how corners are handled:

![img](./figures/fs-7.png)

And the `cap` buttons let you control line ends:

![img](./figures/fs-8.png)

Note that the three lines above have the same endpoints, and differ only in style.

Finally, if you mix fill and stroke (and start/mid/end markers), you can control their exact z-ordering with the last six buttons:

![img](./figures/fs-9.png)

In this figure the same object is drawn twice.
Once with the stroke above the fill (left), and once with the fill above the stroke (right).

### Copy-pasting style

Styles can be copied and pasted!

To do this, select an item, copy it (`Ctrl+V`), select another item, and paste on the style using `Ctrl+Shift+V`.

This is particularly useful after resizing things (which scales line widths too).

![img](./figures/fs-10.png)

For whatever reason, advanced properties such as stroke/fill z-order can not be copied this way.

## Text

Text can be inserted in two ways:

If you select the text tool and click anywhere on the page, you can add text that flows wherever it can.
If instead you drag a box, the text will remain inside the box.

![img](./figures/text-1.png)

Note that the box surrounding the text in the example below has gone red to indicate that the text doesn't fit!

The toolbar that shows up when the text tool is selected lets you change font, font size, line spacing etc.

Working with text in Inkscape can be quite annoying.
For example, the alignment tool sometimes stops working, and sometimes settings don't seem to get applied unless I select all the text first.

