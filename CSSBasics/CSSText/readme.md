# CSS Text:

CSS has a lot of properties for formatting text.Some of its CSS properties are:

1. Text Color:

The `color` property is used to set the color of the text.The color is specified by: a color name, a HEX value & an RGB value. For example:
```css
    color: orange;
    color: rgb(0,120,240)
    /* all the light sources ranges from 0 to 255 */
    color: #12ABFF;
    /* #RRGGBB ,here RR, GG, BB ranges from 00 to FF */
```

2. Text Alignment:

The `text-align` property is used to set the horizontal alignment of a text.A text can be left or right aligned, centered, or justified.For Exapmle:
```css
text-align: left;
text-align: right;
text-aligh: center;
text-aligh: justify;
/* each line is stretched so that every line has equal width and the left & right margins are straight */
```

3. Text Direction:

The `direction` property specifies the text direction / writing direction within a block-level element.
___CSS Syntax:__
```css
direction: ltr|rtl|inital|inherit;
/*
ltr - text direction goes from left to right 
rlt - text direction goes from roght to left
inital - used to set  a property to its default value
inherit - inherit the parent or previous value
``` 

The `unicode-bidi` property is used together with the direction property to set or return whether the text should be overridden to support multiple languages in the same document.
___CSS Syntax:__
```css
unicode-bidi: normal|embed|bidi-override|isolate|isolate-override|plaintext|inital|inherit;
/*
normal - The element does not open an additional level of embedding. This is default

embed - For inline elements, this value opens an additional level of embedding

bidi-override - For inline elements, this creates an override. For block elements, this creates an override for inline-level descendants not within another block element

isolate	- The element is isolated from its siblings	 

isolate-override -

plaintext -

initial	- Sets this property to its default value.

inherit	- Inherits this property from its parent element.
*/
```

4. Text Vertical Alignment:

The vertical-align property sets the vertical alignment of an element.
__CSS Syntax:__
```css
vertical_align: top|middle|bottom;
```

5. Text Docoration:

The `text-decoration` property is used to set or remove decorations from text.
__CSS Syntax:__
```css
text-decoration: none|overline|line-through|underline;
```

6. Text Transformation:

The `text-trensform` property is used to specify uppercase and lowercase letters in text.
__CSS Syntax:__
```css
text-transform:uppercase|lowercase|capitalize;
```

7. Text Spacing:
 
 The `text-indent` property is used to specify the indentification of first line of text.
 __CSS Syntax:__
 ```css
 text-indent: px|em|cm;
 ```

 The `letter-spacing` property is used to specify the space between the characters in a text.
  __CSS Syntax:__
 ```css
 letter-spacing: px|em|cm;
 ```

The `word-spacing` property is used to specify the space between the words in a text.
__CSS Syntax:__
```css
word-spacing: px|em|cm;
```

 The `line-height` property is used to specify the space between lines.
 __CSS Syntax:__
 ```css
 line-height: px|em|cm;
 ```

The `white-space` property specifies how white-space inside an element is handled.
__CSS Syntax:__
```css
white-space: normal|nowrap|pre|pre-line|pre-wrap|initial|inherit;
/*
normal - Text will wrap when necessary.

nowrap - Sequences of whitespace will collapse into a single whitespace. Text will never wrap to the next line. The text continues on the same line until a <br> tag is encountered
*/
```

8. Text Shadow:

The text-shadow property adds shadow to text.
__CSS Syntax:__
```css
text-shadow: h-shadow v-shadow blur-radius color|none|initial|inherit;

/*
h-shadow specifies the horizontal shadow 
v-shadow specifies the vertical shadow
*/
```