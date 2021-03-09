# CSS Paddings:

The CSS `padding` properties are used to generate space around an element's content, inside of any defined borders.CSS has properties for specifying the padding for each side of an element.All the padding properties can have the following values:

- length - specifies a padding in px, pt, cm, etc.
- % - specifies a padding in % of the width of the containing element
- inherit - specifies that the padding should be inherited from the parent element

For Example:
```css
  padding-top: 50px;
  padding-right: 30px;
  padding-bottom: 50px;
  padding-left: 80px;

  /* Shorthand property */
   padding: 50px 30px 50px 80px;
```

```css
/* Here, the <div> element is given a width of 300px. However, the actual width of the <div> element will be 350px (300px + 25px of left padding + 25px of right padding) */
div{
    width: 300px;
    padding: 25px;
}

/* To keep the width at 300px, no matter the amount of padding, you can use the box-sizing property. This causes the element to maintain its width; if you increase the padding, the available content space will decrease. */

div {
    width: 300px;
    padding: 25px;
    box-sizing: border-box;
} 
```