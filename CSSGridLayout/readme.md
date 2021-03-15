> # CSS Grid Layout:

The CSS Grid Layout Module offers a grid-based layout system, with rows and columns, making it easier to design web pages without having to use floats and positioning.For example:
```css
<head>
    <style>
        .grid-container {
            display: grid;
            grid-template-colums: auto auto;
        }
    </style>
</head>
<body>
    <div class="grid-container">
        <div class="grid-item">1</div>
        <div class="grid-item">2</div>
        <div class="grid-item">3</div>
        <div class="grid-item">4</div>
    </div>
</body>
```

An HTML element becomes a grid container when its display property is set to `grid` or `inline-grid`.All direct children of the grid container automatically become grid items.

You can adjust the gap size by using one of the following properties:

- `grid-column-gap`
- `grid-row-gap`
- `grid-gap`

The `grid-template-columns` property specifies the number (and the widths) of columns in a grid layout.The `grid-template-rows` property specifies the number (and the heights) of the rows in a grid layout.

The lines between columns are called column lines.Similarly,the lines between rows are called row lines.The following properties control where to start and end a grid item:

- grid-column-start
- grid-column-end
- grid-row-start
- grid-row-end

For Example:
```css
.item1 {
  grid-column-start: 1;
  /* the grid for that grid-item will start from column-line-one */
  grid-column-end: 3;
  /* the grid for that grid-item will end when it meets column-line-three */
}

.item2 {
  grid-row-start: 1;
  /* the grid for that grid-item will start from row-line-one */
  grid-row-end: 5;
  /* the grid for that grid-item will end when it meets row-line-five */
}

.item3 {
    grid-column: 1 / span 3;
    /* The grid-column property is a shorthand property for the grid-column-start and the grid-column-end properties. */
    /* Item1 will start on column-line 1 and span 3 columns. */
}

.item4 {
    grid-row: 1 / span 3;
    /* The grid-row property is a shorthand property for the grid-row-start and the grid-row-end properties. */
    /* Item1 will start on row-line 1 and span 3 rows. */
}


.item5 {
    grid-area: 1 / 2 / 5 / 6;
    /* The grid-area property can be used as a shorthand property for the grid-row-start, grid-column-start, grid-row-end and the grid-column-end properties. */
    /* Make "item5" start on row-line 1 and column-line 2, and end on row-line 5 and column line 6: */
}
```