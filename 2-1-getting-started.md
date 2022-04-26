# Making diagrams with Inkscape

Inkscape is an open source tool to create vector art.

It uses the SVG format by default, but can open and export to several other formats.

It has some pretty amazing capabilities, but you might also encounter some glaring bugs.

- Use Ctrl+S to save as a matter of habit.
  - (if it does crash, it will sometimes make a back-up first!)
  - SVG is plain text, it works reasonably well with git (but forget about diff'ing, unless you have some kind of XML extension installed).
  - You can bother one of its maintainers on twitter (just use the word "inkscape" and eventually he'll show up).
  - Alternatives are costly (240 a year to adobve, for you [and your collaborators](https://en.wikipedia.org/wiki/Vendor_lock-in)).

![ink](./figures-2/hello.png)

👆 Inkscape's user interface, on a Gnome/Fedora linux OS.



## Setting up inkscape

Incomplete list of things I like to do first:

- Open Document Properties, and set the "Display units" to "mm"
- Set the width to whatever width the journal uses for a 2-column figure
- Set the height to something bigger - you'll adjust this later
- On the "Grids" tab, add a nice rectangular grid e.g. with steps every 0.5mm and a thicker line every 2.5mm
- You can configure your grid as default in "Preferences"
- Another thing to look at in "Preferences" is Behaviour > Steps. Set this to the same as your grid so that arrow keys or Shift+Arrow keys move the objects without going off the grid.
- Make sure you have "snap" settings as in the tutorial above.

- Start with a fixed width. 
  - Use sensible font size e.g. 10.
  - Can even use same font as article?

