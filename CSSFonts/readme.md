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
__CSS Syntax:__
```css
    font-size: px|em|%|vw;
    /* 1 em = 16px; */
    /* vw = veiwport width */
```

### CSS Font Shorthanded:
To shorten the code, it is also possible to specify all the individual font properties in one property called `font`.
__CSS Syntax:__
```css
    font: font-style font-variant font-weight font-size/line-height font-family;
```
For exapmle:
```css
    p {
        font: italic small-caps bold 12px/30px Georgia, serif;
    }
```

### CSS Google Fonts:

If you do not want to use any of the standard fonts in HTML, you can use Google Fonts.

Just add a special style sheet link in the <head> section and then refer to the font in the CSS.
__CSS Syntax:__
```css
<head>
    <link rel="stylesheet" href="url">
    <style>
        font-family: familyName ;
    </style>
</head>
```
For example:
```css
<head>
    <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Sofia">
    <style>
        body {
            font-family: "Sofia", sans-serif;
        }
    </style>
</head>

/* To use multiple Google fonts, just separate the font names with a pipe character (|) */
<head>
    <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Audiowide|Sofia|Trirong">
    <style>
        h1.a {font-family: "Audiowide", sans-serif;}
        h1.b {font-family: "Sofia", sans-serif;}
        h1.c {font-family: "Trirong", serif;}
    </style>
</head>

/* in addition you can style Google Fonts */
<head>
    <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Sofia">
    <style>
        body {
            font-family: "Sofia", sans-serif;
            font-size: 30px;
            text-shadow: 3px 3px 3px #ababab;
        }
    </style>
</head>

/* Google have also enabled different font effects that you can use. */
/* First add "effect=effectname" to the Google API, then add a special class name to the element that is going to use the special effect. The class name always starts with "font-effect-" and ends with the "effectname" */
<head>
    <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Sofia&effect=fire">
    /* adding "effect=fire" */
    <style>
    body {
        font-family: "Sofia", sans-serif;
        font-size: 30px;
    }
    </style>
</head>
<body>

    <h1 class="font-effect-fire">Sofia on Fire</h1>
    /* adding special class called "font-effect-fire" */

</body>

/* To request multiple font effects, just separate the effect names with a pipe character (|) */
<head>
    <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Sofia&effect=neon|outline|emboss|shadow-multiple">
    <style>
    body {
        font-family: "Sofia", sans-serif;
        font-size: 30px;
    }
    </style>
</head>
<body>

    <h1 class="font-effect-neon">Neon Effect</h1>
    <h1 class="font-effect-outline">Outline Effect</h1>
    <h1 class="font-effect-emboss">Emboss Effect</h1>
    <h1 class="font-effect-shadow-multiple">Multiple Shadow Effect</h1>

</body>
```