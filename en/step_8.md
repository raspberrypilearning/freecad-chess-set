## Manufacture the board

There are two ways of making the board: 3D printing or laser cutting.

### 3D printing

--- task ---
For each of your sides and base/top, use the **Part Design** workbench to add a 3mm pad to the sketch.

![PartDesign_Pad](images/PartDesign_Pad.png)

![padded_side](images/padded_side.png)
--- /task ---

--- task ---
Go to the **File** menu to **Export** each piece. Select **STL Mesh** as the file type.
--- /task ---

--- task ---
Print each of the pieces twice, so that you have a base, a top, and four sides.
--- /task ---

### Laser cutting
--- task ---
Open each sketch in the **Sketcher** workbench. Then, go to the **File** menu to **Export** each sketch as a **Flattened SVG**.
--- /task ---

--- task ---
Open each of the SVG files in Inkscape.

![side_svg](images/side_svg.png)

To check that the scale has been maintained, open the **File** menu, go to **Document Properties**, then change the **Units** to `mm`.

![document_properties](images/document_properties.png)
--- /task ---

--- task ---
To alter the **Fill and Stroke** properties, select your sketch, then press <kbd>Shift + Ctrl + F</kbd>.

Different laser cutters require different settings, but most will cut with a stroke width of `0.1`mm and a stroke colour that is `255 Red`.

![stroke_width](images/stroke_width.png)

![stroke_colour](images/stroke_colour.png)

--- /task ---

The file should now be ready to send to the laser cutter. Make sure that that you cut each of the sketches twice.

--- task ---
Optional task:

If you like, you could etch black and white squares into the top of your chessboard before you cut it. To do this, carefully place the below image over the top of the SVG file.

<html>
<a title="Nevit Dilmen [Public domain], via Wikimedia Commons" href="https://commons.wikimedia.org/wiki/File:Chess_Board.svg"><img width="512" alt="Chess Board" src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/d5/Chess_Board.svg/512px-Chess_Board.svg.png"></a>
</html>
--- /task ---

### Print the pieces

--- task ---
Export each chess piece as an STL file, then print the pieces.

This project does not contain instructions for 3D printing because printers vary. However, [Cura](https://ultimaker.com/software){:target="_blank"} and [Octopi](https://octoprint.org/download/){:target="_blank"} are useful pieces of software to slice and print your models.

If you would like to learn more about how to slice and print models using this software, you can [find further instructions here](https://projects.raspberrypi.org/en/projects/getting-started-freecad/7){:target="_blank"} and [here](https://projects.raspberrypi.org/en/projects/getting-started-freecad/8){:target="_blank"}.
--- /task ---
