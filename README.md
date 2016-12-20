#SASS CSS Responsive Custom Grid

Benefits:

* **Clean HTML**: Doesn't require classes on columns. Less markup than bootstrap.
* **Semantic CSS**: You use your own class names
* **Separation of Concerns**: Presentation info is where it should be, inside the CSS
* **Pay to play**: Less CSS than bootstrap<
* **Percentage based gutters**: Ok, not exactly a benefit, but it was the only way I could get it work - I'll chalk it up as a feature :)
 
Grid CSS is pre built using a mixing, like:
````SCSS
  @include grids((
    ('.responsive-four-col-grid', (md:(3, 3, 3, 3), sm:(6, 6, 6, 6))),

    ('.responsive-nested-grid', (md:(4, 4, 4))),
    ('.two-col-grid', (sm:(6, 6))),
  ));
````
