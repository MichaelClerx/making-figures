# Plotting data and functions with Matplotlib


https://english.stackexchange.com/questions/43027/whats-the-difference-between-a-graph-a-chart-and-a-plot

- Matplotlib is amazing, but also a little bit shit.
  - Has two interfaces: A newer object oriented one, and an older matlab based
    one (pyplot). There are hidden disadvantages to pyplot, so best to switch
    to object oriented one (w. exception of figure creation).
  - Naming is massively inconsistent.
  - Docs can be difficult, e.g.
    - E.g. docs for "plot" are under ("pyplot" or) under "Axes", (it's a method
      of the class Axes). But most arguments are under "Line2D" (plot() creates
      a Line2D and passes the ``kwargs`` to its constructor).
- Remember secondary school:
  - Add axes labels before you even type `ax.plot()`
  - You can use latex eq in your labels
  - Add units! You will forget them later :D
  - Add a legend
  - Do these things while designing. Only once you're finished you can think
    about removing some labels (e.g. when repeated vertically/horizontally).
- Plotting lines and markers
  - single arg 'ks--' versus kwargs
  - alpha (but show example where it went wrong! plus EPS!)
  - colours, setting with colourmap
  - line width, style etc. (Leave the same until need to change!)
  - zorder
  - markers
  - drawstyle (steps)
- Axes
  - Limits
  - Ticks, ticklabels
  - Grid
  - Frame
- Legends
  - Frame, alpha
  - Line width, padding etc
  - Columns
  - Positioning (e.g. moving outside of the graph)
    - axes versus data coordinates
  - Custom lines and labels
- Annotations
  - axvline, axhline
  - axvspan, axhspan
  - text
  - shapes
  - Insets
    - axes versus data coordinates
- Page layout
  - Using gridspec and subgridspec
  - Repeated graph? Use same y limits! (also between figures!)
  - removing labels and yticklabels/xticklabels
  - Adding panel labels (A, B, etc.)
  - Padding: wspace & hspace, plus subplots_adjust
- Save as PDF and/or PNG
  - rasterized=True
- Neat tricks:
  - Connecting areas on two different graphs (transformations!)
  - Semi-automatic panel labels (transformations!)
  - Rainbow lines!
