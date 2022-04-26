# General tip 1: Design for papers

### 2.1 Don't design for screen

A very easy way to waste time is to design figures that look good on screen and then adapt them later.
You may even fall in love with your screen-designed figures, making it difficult to let go or have new ideas

### 2.2 Start with a fixed width

The first thing to do when making a figure is setting its width.
(Set the height to something big, and trim down when finished).

In theory, you should look up or measure the widths of 1 column and 2 column figures in the journal guidelines.
In practice, just picking two arbitrary-but-consistent numbers works fine.
This might mean your figures get rescaled a little, but as long as it's consistent between figures this will still look great.

I've used e.g. 80mm for single and 170mm for double column figures, or 3 inches and 7 inches.

### 2.3 Pick a readable font size and use it throughout (e.g. Arial 10)
  
Setting a physical width (in mm or inches) makes the font size a meaningful number.
For paper figures, anything below 8 or 9pt probably won't be readable, and anything bigger than 11.5pt can seem clumsy or oversized.

Be consistent, and use the same fonts, font sizes etc. in all figures of your paper.

### 2.4 Minimise whitespace around your figure

The article typesetter (or software) will take care of padding. Add only the tiniest sliver in your figure file.

## Examples

### A figure designed for screen
![Look at this](./figures-1/one-page-paci-vcp_opt-beat1.png)

I love this figure, but it is much too big (and busy) to go in a paper.

### Fixed widths help you get things right

![fig](./figures-1/fixed-width-good.png)

The figure above was designed to fit in a single column.
As a result, the labels are readable and the line widths are good.
No tweaking was required: just choosing common values (10pt font, 1pt line width) resulted in a readable figure.

<img src="./figures-1/fixed-width-bad.png" width="396" />

A screen-designed figure crammed into the same space.
Obviously you wouldn't publish this, but imagine the work needed to adapt the above figure so that it looked good in print.
You wouldn't just be changing line sizes and fonts, but also redoing the whole layout.
Probably some elements would need removing.
Avoid all this unnecessary work by designing for print from the outset.

"_But if I use vector graphics or a high DPI then people can just zoom in, it's the 21st century etc._".
Sure, and in some cases this is fine. But
- Large figures are difficult to read on phones, tablets, e-readers etc.
- Some scientists are old and/or visually impaired
- Some editors still want the figures to look good in print
- Some journals are still read in print (especially medical ones)

### It's not your job to add padding

![fig](./figures-1/dont-add-padding.png)

Padding gets added in the typesetting phase. Leave it to the typesetter!

