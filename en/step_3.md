## The King

The king is not much more difficult to make than the rook.

--- task ---
Open up your `rook.FCStd` file, and save it again as `king.FCStd`
--- /task ---

--- task ---
Use the *Create a cube solid* icon to place an additional cube into your project
![Part_Box.png](images/Part_Box.png]) 
--- /task ---

This new cube will be the king's *head*, so it needs to be placed on top of the base.

--- task ---
Click on the new cube in the **Model** tab and then in the **Property** tab change the `angle` to `45°`

Then change the position of the cube so that it has an `x` position of `7.5mm` and a `z` position of `15mm`

![kings_head_position](images/kings_head_position.png)
--- /task ---

If you look at the king from the top-down view, you'll notice that the corners of the head do not line up with the edges of the base.

The length of the sides of the cube need to be increased. You can use [Pythagoras' theorem](https://en.wikipedia.org/wiki/Pythagorean_theorem) to calculate the required dimensions of the cube.

The sum of the square of the length of the two blue lines is equal to the square of the lenght of the red line.

<html>
<math>
    <mrow>
      <mrow>
        <msup>
          <mi>a</mi>
          <mn>2</mn>
        </msup>
        <mo>+</mo>
        <msup>
          <mi>b</mi>
          <mn>2</mn>
        </msup>
      </mrow>
      <mo>=</mo>
      <msup>
        <mi>c</mi>
        <mn>2</mn>
      </msup>
    </mrow>
  </math>
</html>

or

<html>
<math>
    <mrow>
      <mrow>
        <msup>
          <mi>a</mi>
          <mn>2</mn>
        </msup>
        <mo>+</mo>
        <msup>
          <mi>b</mi>
          <mn>2</mn>
        </msup>
      </mrow>
      <mo>=</mo>
      <msup>
        <mi>c</mi>
        <mn>2</mn>
      </msup>
    </mrow>
  </math>
</html>
