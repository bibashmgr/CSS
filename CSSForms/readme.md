# CSS Forms:

If you only want to style a specific input type, you can use attribute selectors.For exapmle:
```css
input[type=text] {
    /* styling */
}
```

Use the `:focus` selector to do something with the input field when it gets focus:
```css
input[type=text] {
    border: 1px solid #555;
}

input[type=text]:focus {
    background-color: lightblue;
}
```

Example:
```css
/* animated search input */

input[type=text] {
    width: 0%;
    border: none;
    font-size: 16px;
    background-color: white;
    background-image: url('searchicon.png');
    background-position: 10px 10px; 
    background-repeat: no-repeat;
    padding: 12px 20px 12px 40px;
    transition: width 0.4s ease-in-out;
    cursor: pointer;
}

input[type=text]:focus {
    width: 50%;
    border: 2px solid #ccc;
    border-radius: 4px;
}
```