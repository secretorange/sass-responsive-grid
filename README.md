#SASS CSS Responsive Custom Grid

[Demo on CODEPEN](http://codepen.io/leegunn/pen/QGYYzv/)

Benefits:

* **Clean HTML**: Doesn't require classes on columns. Less markup than bootstrap
* **Semantic CSS**: You use your own class names
* **Separation of Concerns**: Presentation info is where it should be, inside the CSS
* **Pay to play**: Less CSS than bootstrap
* **Percentage based gutters**: Ok, not exactly a benefit, but it was the only way I could get it work - I'll chalk it up as a feature :)
 
First, define your grids using the SASS mixin. You specify the selector (class or ID) and the column definitions for different breakpoints (xxs, xs, sm, md, lg)

````SCSS
  @include grids((
    ('.responsive-four-col-grid', (md:(3, 3, 3, 3), sm:(6, 6, 6, 6))),
    ('.my-grid', (md:(4, 4, 4))),
    ('.my-two-col-grid', (sm:(6, 6))),
  ));
````

Then simply use your grids in your HTML:

```HTML
<div class="responsive-four-col-grid">
  <div>Col One</div>
  <div>Col Two</div>
  <div>Col Three</div>
  <div>Col Four</div>
</div>
```
