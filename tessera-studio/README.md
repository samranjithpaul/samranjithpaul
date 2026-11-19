# Tessera Studio

Tessera Studio turns a photo into a numbered diamond-painting pattern. It runs in your browser and can be used offline after downloading the HTML file.

**Live website** · [Open Tessera Studio](https://tessera-studio-samranjithpauls-projects.vercel.app/)

## What you can do

- Turn portraits, pet photos, or illustrations into patterns for a physical diamond-painting canvas.
- Generate a grid from your canvas measurements and bead spacing, then preview the mosaic before printing.
- Use the bead counts to plan materials and the numbered placement guide to assemble the design.

## Use it

1. Open the live app, or download and open `index.html` in a browser.
2. Choose a JPG, PNG, or WebP photo up to 20 MB, or try the sample artwork.
3. Enter your usable canvas width and height in centimeters. Measure the spacing between bead cell centers in millimeters. For a more accurate measurement, measure across ten cell intervals and divide by ten.
4. Set the color limit, palette, and photo fit, then select **Generate pattern**.
5. Switch to **Numbered placement** to see where each bead goes. Match the generated color swatches to your physical beads.

## Downloads

| File | Contents |
| --- | --- |
| Placement PDF | A4 pages with the section map, numbered placement grid, bead legend, and color counts |
| Preview PNG | Image of the finished mosaic |
| Bead list CSV | Bead number, hex color, and quantity |

Print the PDF on A4 at **Actual size (100%)** and check that the calibration ruler measures 50 mm. Start from the top-left of your canvas and align the sections using the row and column numbers. The grid rounds down to whole cells.

## Tech stack

- **HTML** for the page and controls
- **CSS** for the responsive layout
- **Vanilla JavaScript** for photo processing, color reduction, and exports
- **Canvas API** for the mosaic preview and numbered placement view

Everything is in `index.html`. There is no build step, backend, or API key. Photo processing and file generation happen on your device.
