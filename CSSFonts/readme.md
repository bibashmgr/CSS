# CSS Fonts:

In CSS there are five generic font families:

1. Serif fonts: They have a small stroke at the edges of each letter. They create a sense of formality and elegance.
2. Sans-serif fonts: They have clean lines (no small strokes attached). They create a modern and minimalistic look.
3. Monospace fonts: Here, all the letters have the same fixed width. They create a mechanical look. 
4. Cursive fonts: It imitate human handwriting.
5. Fantasy fonts: They are decorative/playful fonts.

### CSS Font Family:
In CSS, we use the `font-family` property to specify the font of a text.The `font-family` property should hold several font names as a "fallback" system, to ensure maximum compatibility between browsers/operating systems.This means that you should add a list of similar "backup fonts" in the font-family property. If the first font does not work, the browser will try the next one, and the next one, and so on. Always end the list with a generic font family name. Start with the font you want, and end with a generic family (to let the browser pick a similar font in the generic family, if no other fonts are available). The font names should be separated with comma.
For Example:
```css
.p1 {
  font-family: "Times New Roman", Times,  serif;
  /* Here, there are three font types: Times New Roman, Times and serif. The second and third fonts are backups, in case the first one is not found. */
}

.p2 {
  font-family: Georgia, serif; 
}

.p3 {
  font-family: Garamond, serif;
}

.p4 {
  font-family: Arial, Helvetica, sans-serif;
}

.p5 {
  font-family: Tahoma, Verdana, sans-serif;
}

.p6 {
  font-family: "Trebuchet MS", Helvetica, sans-serif;
}

.p7 {
  font-family: "Lucida Console", "Courier New", monospace;
}

.p8 {
  font-family: "Brush Script MT", cursive;
}

.p9 {
  font-family: Copperplate, Papyrus, Fantasy;
}
```

### CSS Font Style:

The `font-style` property is mostly used to specify italic text.
__CSS Syntax:__
```css
font-style: normal|italic|oblique;
```

The `font-weight` property specifies the weight of a font.
__CSS Syntax:__
```css
font-weight: normal|lighter|bold|length(num);
```

The `font-variant` property specifies whether or not a text should be displayed in a small-caps font.
__CSS Syntax:__
```css
font-variant: normal|small-caps;
```

### CSS Font Size:

The `font-size`property sets the size of the text.

