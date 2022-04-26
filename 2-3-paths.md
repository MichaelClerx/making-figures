# Inkscape: Paths

Let's draw an ion current!
In particular, let's redraw something like the top-left figure in [this image](https://github.com/pints-team/pints/blob/master/example.svg).

Select the line tool, and draw a path consisting of two line segments:

![img](./figures-2/ion-1.png)

Now select the `Edit path by nodes` tool, and select the path you just drew.

![img](./figures-2/ion-2.png)

Click the center of a line segment, and drag it along a bit!
Do this for both lines:

![img](./figures-2/ion-3.png)

Hurray! We've turned our straight line into a [Bezier curve](https://en.wikipedia.org/wiki/B%C3%A9zier_curve).

The current selection shows 3 "nodes", connected by 2 "segments".
If we click one of the line segments again, Inkscape will also show the "handles" at each node (lines ending in open circles).
You can move these about to mess with the curvature:

![img](./figures-2/ion-4.png)

Like nodes, handles can "snap" to the grid, so that we can set them systematically.
At each end, the line segment will be tangential to its handles.
In between, the curvature varies smoothly, at a rate set by the ratio between the handle lengths.

We can mess around a bit until we have something almost acceptable:

![img](./figures-2/ion-5.png)

To make it look more like an ion current, we'll need to move the middle point a bit more towards the left.

This can be fiddly!
If you select a line segment, and then drag a node, the whole line segment will move!
If you end up in this situation, undo with `Ctrl+Z`, and then click the node first to select it.
Now you should be able to move just the node (and its handles).

![img](./figures-2/ion-6.png)
On the left, the whole line segment is selected.
On the right, only the middle node is selected.

Move the node a bit to the left, and adjust the handles, to get something that looks more like an ion current.
If you want, move the top-right node too, to add a non-zero steady state current.

![img](./figures-2/ion-7.png)

This is better, but the right segment still doesn't look quite right.
We can try adding more detail by adding a new point.
Select the right segment, and click `Insert new nodes into line segment`, top-left in the toolbar.

![img](./figures-2/ion-8.png)

This gives us some extra degrees of freedom to play with.
If your Inkscape is set up like mine, there will be an interesting difference between the new node and the previous ones: both handles have the same curvature!
The buttons highlighted below let you adapt this behaviour per node:

![img](./figures-2/ion-9.png)

- corner: Both handles are indepdent, letting you can make sharp edges.
- smooth: Both handles have the same curvature, letting you make smooth curves.
- symmetric: Both handles have the same curvature and length.
- auto-smooth: Like smooth, but smooths the curve for you any time you click it.

"Corner" and "smooth" are most useful for our purposes.

The buttons to the left are also worth exploring.
These let you add nodes, delete line segments between nodes, etc.

After some messing about (you may want to disable snapping during this), you might find a nice curve.
Or you may find that it was easier without this new point!
No worries, just delete it again by selecting and hitting the `Delete selected nodes` button next to the `Insert nodes` one.

Maybe if we try tracing an existing image?
Click `File > Import`, find the file `ina.png` in this repo, and double click to open.
Inkscape will ask you if you want to embed or link to this file.
Usually you'll want to embed (meaning the image will be stored as part of the SVG file), but for now it doesn't matter: we'll delete this imported file again in a few moments.

Now we've created a raster/vector hybrid!
Use the Z-index buttons near the top to move the raster image underneath our line.
Next, resize the image until it approximately fits.

![img](./figures-2/ion-10.png)

Maybe it wasn't such a bad effort after all.
Make a few tweaks and delete the image again.

Now let's use some of Inkscape's crazier features.

First, we'll need a back up.
Select the cursor tool, click your path, and use `Ctrl+C` and `Ctrl+Alt+V` to create a copy in place.
Use `Shift+Arrow keys` to move the copy down.

Now go to `Extensions > Modify path > Add nodes`.

![img](./figures-2/ion-11.png)

Select `By max. segment length` and `Maximum segment length(px): 0.1`, and hit `Apply`.

![img](./figures-2/ion-12.png)

Now reselect the `Edit path` tool to see what you have done:

![img](./figures-2/ion-13.png)

Now got to `Extensions > Modify path > Jitter`.
Set a maximum x displacement of 0, and set y to e.g. `3.0 px`.
Make sure `Distribution` is set to `Gaussian` and hit `Apply`.

![img](./figures-2/ion-14.png)

Switch back to the cursor tool and use `Shift+Arrow keys` to make the curve overlap with our back-up.
Use the z-index controls to make sure the noisy curve is behind the smooth one, and set some nice stroke colours for each.
You may also want to reduce the stroke size of the noisy curve.

![img](./figures-2/ion-15.png)

Congratulations! You've fitted an ion current 🤔

