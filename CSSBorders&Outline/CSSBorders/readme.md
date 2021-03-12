# CSS Borders:

The CSS border properties allow you to specify the style, width, and color of an element's border.

1. CSS Border Style:

The `border-style` property specifies what kind of border to display.

The following values are allowed:

- dotted - Defines a dotted border
- dashed - Defines a dashed border
- solid - Defines a solid border
- double - Defines a double border
- groove - Defines a 3D grooved border.
- ridge - Defines a 3D ridged border.
- inset - Defines a 3D inset border.
- outset - Defines a 3D outset border.
- none - Defines no border
- hidden - Defines a hidden border

You can use a mixed border too.For example:
```css
border-style-top: dotted;
border-style-right: dashed;
border-style-bottom: solid;
border-style-left: double;

/* short-handed way */
border-style: dotted dashed solid double;
```

2. CSS Border Width:

The `border-width` property specifies the width of the four borders.The width can be set as a specific size (in px, pt, cm, em, etc) or by using one of the three pre-defined values: thin, medium, or thick.The `border-width` property can have from one to four values (for the top border, right border, bottom border, and the left border).For Example:
```css
  border-width: 5px ; 
  /* 5px on the all sides */

  border-width: 5px 20px; 
  /* 5px on top and bottom, 20px on the sides */

  border-width: 20px 5px 15px; 
  /* 20px on top, 5px on the sides, 15px on bottom */

  border-width: 5px 20px 10px 15px; 
  /* 5px on top, 20px on right, 10px on bottom and 15px on left */
```

3. CSS Border Color:

The `border-color` property is used to set the color of the four borders.The `border-color` property can have from one to four values (for the top border, right border, bottom border, and the left border).For Example:
```css
  border-color: red ; 
  /* red on the all sides */

  border-width: red green; 
  /* red on top and bottom, green on the sides */

  border-width: red green blue; 
  /* red on top, green on the sides, blue on bottom */

  border-width: red green blue black; 
  /* red on top, green on right, blue on bottom and  black on left */
```

## CSS Shorhanded Border property:
The `border` property is a shorthand property for the following individual border properties:

- `border-width`
- `border-style`
- `border-color`

For example:
```css
border: 1px solid red;
/* sets the border of an element with solid style ,red color border and 1px width. */

border-left: 5px dotted green;
/* sets the border of an element on left side with dotted style ,green color border and 5px width. */
```

## CSS Rounded Borders:
The `border-radius` property is used to add rounded borders to an element.For example:
```css
  border: 2px solid red;
  border-radius: 5px;
```
