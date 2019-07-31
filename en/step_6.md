## Make the bishops

The bishops are the most difficult pieces to make. Instead of trying to make them out of primitive pieces, you will use a **Sketch** to describe the shape, then turn this into a 3D piece.

--- task ---
Create a new file, then go to the workbench menu and select **Part Design**.

![part_design](images/part_design.png)
--- /task ---

--- task ---
Click on the **Create a new body and make it active** icon, then click on the **Create a new sketch** icon.

![PartDesign_Body_Create_New](images/PartDesign_Body_Create_New.png)

![Sketcher_NewSketch](images/Sketcher_NewSketch.png)
--- /task ---

--- task ---
You will be prompted to select a plane, onto which your new sketch will be mapped. Select the **XY_Plane**, then click on **OK**.

![plane_select](images/plane_select.png)
--- /task ---

Your workbench will now change to the **Sketcher** workbench.

First, you will make a **Construction Geometry**. Think of this as a guideline to help you draw an accurate sketch.

--- task ---
To start, click on the **Create a square by its center and by one corner** icon.

![create_square](images/create_square.png)

Hover your cursor over the centre of the XY_Plane, so that the red dot in the middle turns yellow.

![yellow_dot.png](images/yellow_dot.png)

Then, click on the yellow dot and drag outwards to draw a square. This square will be bound to the centre of the plane.

![square_undefined](images/square_undefined.png)
--- /task ---

Next, you will add some **constraints** to the sketch. This will ensure that it is positioned and orientated correctly, with a defined size. 

Look at the **Tasks** tab. You will see that the square already has some constraints on it.

![constraints](images/constraints.png)

Most of these constraints relate to the nature of a square. For example, opposite sides must be parallel and all sides must have the same length. You added one more constraint when you made sure that the square was in the centre of the plane.

In the **Tasks** tab, you will also see that your square has **2 degrees of freedom**.

![degrees_freedom](images/degrees_freedom.png)

This means that you need two additional constraints to fully define the square.

--- task ---
Click on an edge of the square and drag it around. You should see that the square can rotate.

Click on any of the square's edges, then click on the **Create a horizontal constraint in the selected item** icon.

![Constraint_Horizontal](images/Constraint_Horizontal.png)

Now, the square can't rotate anymore.
--- /task ---

--- task ---
If you click on an edge and drag it around now, the square will resize.

Click on a vertical edge, then click on the **Fix the vertical distance between two points or line ends** icon. (It may be in the drop-down menu for the constraints.) Set the **Length** of the edge to `15mm`.

![Constraint_VerticalDistance](images/Constraint_VerticalDistance.png)
--- /task ---

You should see that your square has turned green, and in the **Tasks** tab, there should be a message that says that the sketch is fully constrained.

![fully_constrained_square](images/fully_constrained_square.png)

--- task ---
To turn this square into a construction geometry, select each of the edges and click on the **Toggle construction geometry** icon.

![Sketcher_AlterConstruction](images/Sketcher_AlterConstruction.png)
--- /task ---

The square will turn blue.

![construction_geometry](images/construcion_geometry.png)

--- task ---
Use the **Create a line in a sketch** tool to create four diagonal lines within the square. Make sure that your lines are constrained to the construction geometry.

![Sketcher_CreateLine](images/Sketcher_CreateLine.png)

To ensure that the ends of the lines are constrained, you can hover over the construction geometry so that the lines turn yellow.

![diagonal_lines](images/diagonal_lines.png)
--- /task ---

Sometimes, adding lines can add unnecessary constraints to the sketch. To avoid this, you can draw lines anywhere in the sketch and then constrain them afterwards.

--- task ---
First, draw a small line anywhere in the sketch, so that it is not constrained.

![stray_line](images/stray_line.png)
--- /task ---

--- task ---
Then, use the **Create a coincident constraint** tool to constrain the end points of the line, so that it joins the corner of the construction geometry with the end point of the diagonal line.

![Constraint_PointOnPoint](images/Constraint_PointOnPoint.png)

![constrained_line](images/constrained_line.png)
--- /task ---

--- task ---
Repeat this another seven times to create a sketch that looks like a pointed cross.

![pointed_cross](images/pointed_cross.png)
--- /task ---

--- task ---
Select each of the eight lines that you have just drawn, and create **equality constraints** between them.

![Constraint_EqualLength](images/Constraint_EqualLength.png)
--- /task ---

--- task ---
Now use the **Vertical distance constraint** tool to set the **Length** of one of the vertical lines to `3mm`.

![Constraint_VerticalDistance](images/Constraint_VerticalDistance.png)

Your sketch should become fully constrained, and should turn completely green. If it is not fully constrained, then move some of the points around to find out where you have unconstrained points.

![fully_constrained_square_cross](images/fully_constrained_square_cross.png)
--- /task ---

--- task ---
To finish the sketch, you need to remove some of the lines in the centre of the cross.

Click on the **Trim** icon, then click on the lines in the centre that make up a small square. This will remove them.

![Sketcher_Trimming](images/Sketcher_Trimming.png)

![fully_constrained_cross](images/fully_constrained_cross.png)
--- /task ---

--- task ---
Click on **Close** in the **Tasks** tab. This will take you back to the **Part Design** workbench.
--- /task ---

--- task ---
Make sure that your sketch selected, then use the **Pad** tool to turn the sketch into a 3D object and set the height to `15mm`.

![PartDesign_Pad](images/PartDesign_Pad.png)

![bishop](images/bishop.png)
--- /task ---
