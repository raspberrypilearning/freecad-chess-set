## Bishops

The bishops are the trickiest pieces to make. Rather than trying to make them out of primitive pieces, you're going to use a **Sketch** to describe the shape, and then turn this into a 3D piece.

--- task ---
Create a new file and then switch the workbench to **Part Design**

![part_design](images/part_design.png)
--- /task ---

--- task ---
Click on the icon to **Create a new body and make it active** and then on **Create a new sketch**

![PartDesign_Body_Create_New](images/PartDesign_Body_Create_New.png)

![Sketcher_NewSketch](images/Sketcher_NewSketch.png)
--- /task ---

--- task ---
You will be prompted to select a plane, onto which your new sketch will be mapped, so select the `XY_Plane` and click `OK`.

![plane_select](imagesplane_select.png)
--- /task ---

You will notice that your workbench changes to the **Sketcher** workbench.

You'll start by making what is called a **Construction Geometry**. Think of these as guide lines, to help you draw an accurate sketch.

--- task ---
Start by using the **Create a square by it's center and by one corner**. You'll want to centre your cursor over the centre of the XY_Plane, so that the red dot in the middle turns yellow.

![yellow_dot.png](images/yellow_dot.png)

Then click and drag outwards to draw the square. This square will be bound to the centre of the plane

![square_undefined](images/square_undefined.png)
--- /task ---

Next you're going to add some *constraints* to the sketch. This will ensure that it is positioned and orientated correctly, with a defined size. 

You'll notice that in the **Tasks** tab that the square already has some constraints on it.

![constraints](images/constraints.png)

Most of these constraints are to do with the nature of a square. Opposite sides must be parallel and all sides must have the same length, for instance. One constraint you added yourself, by ensuring the square was in the centre of the plane.

You can also see in the **Tasks** tab that your square has *2 degrees of freedom*

![degrees_freedom](degrees_freedom.png)

This means that you need two additional constraints to fully define the square.

--- task ---
Click on an edge of the square and drag it around. You should see that the square can rotate.

Click on any of the squares edges, then use the **Create a horizontal constraint in the selected item** tool.

![Constraint_Horizontal](images/Constraint_Horizontal.png)

Now the square can't rotate.
--- /task ---

--- task ---
Clicking on an edge and dragging it around, will now cause the square to resize.

Click on an vertical edge and this time use the **Fix the vertical distance between two points or line ends** tool. (It may be in the drop down menu for the constraints. Set the edge length to `15mm`.

![Constraint_VerticalDistance](images/Constraint_VerticalDistance.png)
--- /task ---

You should see that your square has turned green and the the **Tasks** tab there will be a message saying that the sketch is fully constrained.

![fully_constrained_square](fully_constrained_square.png)

--- task ---
To turn this square into a construction geometry, select each of the edges and click on the **Toggle construction geometry** icon.

![Sketcher_AlterConstruction](images/Sketcher_AlterConstruction.png)
--- /task ---

The square should turn blue.

![construction_geometry](images/construcion_geometry.png)

--- task ---
Use the **Create a line in a sketch** tool, to create four diagonal lines within the square. Make sure you're lines are constrained to the construction geometry.

![Sketcher_CreateLine](image/Sketcher_CreateLine.png)

You can ensure the ends of the lines are constrained by hovering over the construction geometry so that the lines turn yellow.

![diagonal_lines](images/diagonal_lines.png)
--- /task ---

Sometimes adding lines can add unnecessary constraints to the sketch. To avoid this you can draw lines anywhere in the sketch and then constrain them afterwards.

--- task ---
Draw a small line, anywhere in the sketch, so it's not constrained.

![stray_line](images/stray_line.png)
--- /task ---

--- task ---
Use the **Create a coincident constraint** tool to constrain the end points of the line, so that it joins to corner of the construction geometry with the end point of the diagonal line.

![Constraint_PointOnPoint](images/Constraint_PointOnPoint.png)

![constrained_line](images/constrained_line.png)
--- /task ---

--- task ---
Repeat this another seven times to create a *pointed cross*-like sketch.

![pointed_cross](images/pointed_cross.png)
--- /task ---

--- task ---
Select each of the eight lines you have just drawn, and create **equality constraints** between them.

![Constraint_EqualLength](images/Constraint_EqualLength.png)
--- /task ---

--- task ---
Now use the **Vertical distance constraint to set the length of one of the vertical lines to 3mm.

![Constraint_VerticalDistance](images/Constraint_VerticalDistance.png)

Your sketch should become fully constrained - turning completely green. If not, then move some of the points around to discover where you have unconstrained points.

![fully_constrained_square_cross](images/fully_constrained_square_cross.png)
--- /task ---

--- task ---
To finish the sketch you need to remove some of the lines in the centre of the cross.

Use the **Trim** tool and click on the lines in the centre that make up a small square.

![Sketcher_Trimming](images/Sketcher_Trimming.png)

![fully_constrained_cross](images/fully_constrained_cross.png)
--- /task ---

--- task ---
Click on **Close** in the Tasks tab, to go back to the **Part Design** workbench.
--- /task ---

--- task ---
With your sketch selected, use the **Pad** tool to turn the sketch into a 3D object, with a height of `15mm`

![PartDesign_Pad](images/PartDesign_Pad.png)

![bishop](images/bishop.png)
--- /task ---
