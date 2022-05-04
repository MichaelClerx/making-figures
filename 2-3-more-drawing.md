# Inkscape: More drawing

## Drawing on a grid

Using the grid lets you easily draw shapes that are similar sizes, and look "tidy", if not very artistic.

![img](./figures-2/shapes.png)

## Going off the grid

To draw more complex shapes, we can use the snapping feature.

In the example below I've drawn a plus sign on the grid, then disabled snap-to-grid before resizing and moving it.

![img](./figures-2/shapes-3d-1.png)

We'll now make a 3d shape.
First, copy the plus sign and move it about a bit.
I've given the plus a white fill to hide what's behind it.

![img](./figures-2/shapes-3d-2.png)

Now, make sure that snapping to "cusp nodes" is enabled, and draw a squinty rectangle connecting the two plus signs:

![img](./figures-2/shapes-3d-3.png)

Do the same thing to create a "side".
I've used different stroke colours to differentiate tops and sides from the original plus.

![img](./figures-2/shapes-3d-4.png)

For the remaining two parts we need something slightly more complicated.
Select "Snap to path intersections" from the snapping toolbar and add in the shape top-right...

![img](./figures-2/shapes-3d-5.png)

...and bottom left.
You can now delete the plus at the back (it's fully obscured by the other shapes), and use `Ctrl+Shift+V` to give all parts the same style.

![img](./figures-2/shapes-3d-6.png)

Finally, choose a strong fill colour for the plus in the front.
Then use the "S" or "V" controls to select a weaker colour for the sides, and one for the tops.

![img](./figures-2/shapes-3d-7.png)

There's more snapping options, e.g. snapping to object centers:

![img](./figures-2/shapes-3d-8.png)

## Distribute and align

The "Align and Distribute" dialog lets you change objects positions (to distribute or align them).
Open it by selecting `Object > Align and Distribute` from the menu, or with `Ctrl+Shift+A`.

In the example below I've made three copies of a circle (without using the grid).

![img](./figures-2/distr-1.png)

Select them all and click `Center on horizontal axis`:

![img](./figures-2/distr-2.png)

Note the `Relative to: first selected` setting in the dialog.
I selected the circle on the left first, so all circles get its y coordinate.

Next, `Distribute centers equidistantly horizontally`:

![img](./figures-2/distr-3.png)

You can use the same tools to place text in the center of objects, but it doesn't always work brilliantly (for short texts the object's center doesn't match its visual centre very well).
Before tweaking:

![img](./figures-2/distr-4.png)

And after some tweaking with the left & right arrows:

![img](./figures-2/distr-5.png)

Use `Alt+Arrow key` to make very small adjustments.

## Example: Drawing a kinetic scheme

We'll now draw a little kinetic scheme (or "Markov model"), starting from the sketch below:

![img](./figures-2/markov-1.jpg)

![img](./figures-2/markov-2.png)

- Start with letters in a reasonable font: these give you a scale!

