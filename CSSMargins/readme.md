# CSS Margins:

Margins are used to create space around elements, outside of any defined borders.CSS has properties for specifying the margin for each side of an element: `margin-top`, `margin-right`, `margin-bottom` & `margin-left`.
All the margin properties can have the following values:
- `auto` - the browser calculates the margin
- `length` - specifies a margin in px, pt, cm, etc.
- `%` - specifies a margin in % of the width of the containing element
- `inherit` - specifies that the margin should be inherited from the parent element

To shorten the code, it is possible to specify all the margin properties in one property.i.e `margin`
```css
margin: 25px 50px 75px 100px;
/* 
top margin is 25px
right margin is 50px
bottom margin is 75px
left margin is 100px
*/
```

## Margin Collapse:

Sometimes two margins collapse into a single margin.Top and bottom margins of elements are sometimes collapsed into a single margin that is equal to the largest of the two margins.This does not happen on left and right margins! Only top and bottom margins.For example:
```css
h1 {
  margin: 0 0 50px 0;
}

h2 {
  margin: 20px 0 0 0;
}
/*
In this example the h1 element has a bottom margin of 50px and the h2 element has a top margin of 20px. So, the vertical margin between h1 and h2 should have been 70px (50px + 20px). However, due to margin collapse, the actual margin ends up being 50px.
*/
```