> # Introduction To CSS:

- CSS stands for Cascading Style Sheets.
 - CSS describes how HTML elements are to be displayed on screen, paper, or in other media.

- CSS saves a lot of work. It can control the layout or style of multiple web pages all at once by creating just an external stylesheet file.

- A CSS rule-set consists of a selector and a declaration block:

     __SYNTAX__:
    ```css
    selector {
        property01 : value01 ; /*Declaration01*/
        property02 : value02 ; /*Declaration02*/
        .
        .
        .
    }
    ```

    - The `selector` points to the HTML element(or group of HTML elements) you want to style.

    - The `declaration block` contains one or more declarations separated by semicolons.

    - Each `declaration` includes a CSS property(attribute) name and a value, separated by a colon.

    - Multiple CSS `declarations` are separated with semicolons, and `declaration blocks` are surrounded by curly braces.

    - There are many types of selectors.They are:

        1. element selector:
            
            It selects HTML elements based on the element name.
        2. id selector:

            It uses the id attribute of an HTML element to select a specific element. To select an element with a specific id, write a hash (#) character, followed by the id of the element.

        3. class selector:

            It selects HTML elements with a specific class attribute. To select elements with a specific class, write a period (.) character, followed by the class name.

        4. universal selector:

            It selects all HTML elements on the page. All you have to use a `*` to select all the elements in the HTML document.

        5. grouping selector:

            It selects all the HTML elements with the same style definitions(i.e Declaration block). To group selectors, separate each selector with a comma.