# css-floating-label
A purley CSS solution for floating label that only appears after the corresponding input's placeholder disappears.
<h3>Usage</h3>

```
<link rel="stylesheet" href="floating.css">

<div class="lbl-float lbl-float-sticky lbl-float-shrink">
  <input type="text" name="myInput" placeholder="My Input Text">
  <label for="myInput">My Input</label>
</div>
```

<p>The input and corresponding label can be added inside a div. <b>The order of the elements is critical: Input first then label.</b></p>
<p>The div element has to have the <b>lbl-float</b> class associated with it. When loaded, the label is hidden and the placeholder is visible. After text is entered, visibility is reversed.</P>
<p>By default, the label appears only when the input has focus. Including the optional <b><i>lbl-float-sticky</i></b> class will continue to display the label after input loses focus (as long as placeholder is not visible)</P>
<p>The <b><i>lbl-float-shrink</i></b> class is optional as well. By default, the div is the height of both elements; using "shrink" will force the div to shrink to the height of the input alone when label is not showing and grow when the label is visible.</p>
