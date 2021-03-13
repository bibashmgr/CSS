# CSS Tables:

To specify table borders in CSS,use the `border` property.For example:
```css
table,  th, td {
    border: 1px solid black;
}
```

To set the width for the table,you can use `width` property.For example:
```css
table {
    width: 100%;
}
```

Similarly, you can the set the height for table or table headings or table data by using `height` property:
```css
th {
    height: 75px;
}

td {
    height: 40px;
}
```

To remove borders, you can use `border-collapse` property which collapsed the double borders into a single border.For example:
```css
table {
    border-collapse: collapse;
} 
```

The `border-spacing` property sets the distance between the borders of adjacent cells.This property works only when `border-collapse` is separate.For example:
```css
#table1 {
    border-collapse: separate;
    border-spacing: 15px;
}

#table2 {
  border-collapse: separate;
  border-spacing: 15px 50px;
  /*
    Using two values (the first sets the horizontal spacing and the second sets the vertical spacing).
  */
}
```

You can sets the horizontal alignment for the content in table-heading i.e `<th>` or table-data i.e `<td>`by using `text-align` property.
__CSS Syntax:__
```css
text-align: left|center|right;
```

For example:
```css
th {
    text-align:center;
}
```

Similarly,You can sets the vertical alignment for the content in table-heading i.e `<th>` or table-data i.e `<td>`by using `vertical-align` property.
__CSS Syntax:__
```css
vertical-align: top|middle|bottom;
```

For example:
```css
th {
    vertical align: middle;
}
```

To control the space between the border and the content in a table,you can use the `padding` property on `<td>` and `<th>` elements.For example:
```css
th, td {
  padding: 15px;
}
```

You can use the `:hover` selector on <tr> to highlight table rows on mouse over.For example:
```css
tr:hover {background-color: #f5f5f5;}
```

You can use the nth-child() selector to style a certain row of the table.For Example:
```css
tr:nth-child(2) {background-color: #f2f2f2;}
```

Add a container element (like `<div>`) with `overflow-x:auto` around the `<table>` element to make it responsive:
```css
<div style="overflow-x:auto;">

    <table>
        /*
        ... table content ...
        */
    </table>

</div>
```

The `caption-side` property specifies the placement of a table caption.
__CSS Syntax__
```css
caption-side: top|bottom|initial|inherit;
```

The `empty-cells` property sets whether or not to display borders on empty cells in a table. This property has no effect if `border-collapse` is "collapse".
__CSS Syntax:__
```css
    empty-cells: show|hide|initial|inherit;
```

The `table-layout` property defines the algorithm used to lay out table cells, rows, and columns.
__CSS Syntax:__
```css
    table-layout: auto|fixed|initial|inherit;
```