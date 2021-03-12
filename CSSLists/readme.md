# CSS Lists:

The CSS list properties allow you to:

- Set different list item markers for ordered lists
- Set different list item markers for unordered lists
- Set an image as the list item marker
- Add background colors to lists and list items

Some of its CSS properties are:

1. `list-style-type`: 
The `list-style-type` property specifies the type of list item marker.
__CSS Syntax:__
```css
    /* unordered list */
    list-style-type: none|circle|square|disc;
    /* ordered list */
    list-style-type: none|upper-roman|lower-roman|upper-alpha|lower-alpha|lower-greek|armenian|georgian|lower-latin|upper-latin;
```

2. `list-style-image`:
The `list-style-image` property specifies an image as the list item marker.
__CSS Syntax__
```css
    list-style-image: url('imageName');
```

3. `list-style-position` 
The `list-style-position` property specifies the position of the list-item markers.
__CSS Syntax__
```css
    list-style-position: outside|inside;
    /* 
    "list-style-position: outside;" means that the bullet points will be outside the list item. The start of each line of a list item will be aligned vertically. 
    
    "list-style-position: inside;" means that the bullet points will be inside the list item. As it is part of the list item, it will be part of the text and push the text at the start.
    */
```

### CSS List shorthand property:

The list-style property is a shorthand property. It is used to set all the list properties in one declaration.
__CSS Syntax__
```css
list-style: list-style-type list-style-position list-style-image;
```