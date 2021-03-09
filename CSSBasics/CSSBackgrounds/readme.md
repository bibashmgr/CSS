# CSS Backgrounds:

The CSS background properties are used to add background effects for elements.Some of CSS background properties:

- background-color:
    The background-color property specifies the background color of an element.

    __Example:__
    ```css
    body {  
        background-color: lightblue;
        opacity: 0.3;
    }
    ```

- background-image:
    The background-image property specifies an image to use as the background of an element.
    By default, the image is repeated so it covers the entire element.
    __Example:__
    ```css
    body {
    background-image: url("background.jpg");
    }
    ```

- background-repeat:
    By default, the background-image property repeats an image both horizontally and vertically.
    __Example:__
    ```css
    /* If the image above is repeated only horizontally */
    body {
    background-image: url("background.jpg");
    background-repeat: repeat-x;
    }
    
    /* If the image above is repeated only vertically */
    body {
    background-image: url("background.jpg");
    background-repeat: repeat-y;
    }

    /* If the image above isnot repeated or you want to show the image once*/
    body {
    background-image: url("background.jpg");
    background-repeat: no-repeat;
    }
    ```

- background-attachment:
    The background-attachment property specifies whether the background image should scroll or be fixed.
    
    __Example:__
    ```css
    body {
    background-image: url("backgorund.jpg");
    background-repeat: no-repeat;
    background-position: right top;
    background-attachment: fixed;
    /* the background image is fixed */
    }
    ```
    ```css
    body {
    background-image: url("backgorund.jpg");
    background-repeat: no-repeat;
    background-position: right top;
    background-attachment: scroll;
    /* the backgrround image is scrollable,meaning when scrolling the page the image will be scrolled too.
    }
    ```

- background-position:
    The background-position property is used to specify the position of the background image.

    __Example:__
    ```css
    body {
    background-image: url("background.jpg");
    background-repeat: no-repeat;
    background-position: right top;
    }
    ```
- background:
    To shorten the code, it is also possible to specify all the background properties in one single property. This is called a shorthand property.

    __Example:__
    ```css
        body {
    background: #ffffff url("img_tree.png") no-repeat right top;
    }
    ```