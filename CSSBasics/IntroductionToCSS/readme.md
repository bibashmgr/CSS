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

# How To Add CSS:

There are three ways of inserting a style sheet:

1. Inline CSS:
    To use inline styles, add the `style` attribute to the relevant element.

    __Example:__
    ```css
    <p style="color:red; border: 1px red solid;">
    ```

2. Internal CSS:
    To use internal styles, add the `<style>` element inside the `<head>` section and defined the css property inside it.

    __Example:__
    ```css
    <head>
        <style>
            body{
                background-color: red;
                color: white;
            }
        </style>
    </head>
    ```

3. External CSS:
    To use external styles, a external .css file is created where all css styling is done.You have to link the HTML document and .css file using `<link>` element.

    __Example__:
    ```html
        <!-- test.html -->
        <head>
            <link rel="stylesheet" href="style.css">
        </head>
    ```

    ```css
        /* style.css */
        body{
            background-color: light-blue;
        }
    ```
# CSS Comments:

Comments are ignored by browsers.A CSS comment starts with /* and ends with */.

__Example:__
```css
/* this is a comment */
```

