# CSS Links:

With CSS, links can be styled in many different ways.Links can be styled with any CSS property (e.g. `color`, `font-family`, `background`, etc.).

In addition, links can be styled differently depending on what state they are in.The four links states are:

1. a:link - a normal, unvisited link
2. a:visited - a link the user has visited, (i.e visted link)
3. a:hover - a link when the user mouses(or hovers) over it
4. a:active - a link the moment it is clicked (i.e selected link)


__Notes:__
When setting the style for several link states, there are some order rules:

- a:hover MUST come after a:link and a:visited
- a:active MUST come after a:hover

ORDER TO FOLLOW WHILE STYLING;
a:link -> a:visted -> a:hover -> a:active