# CSS Animations:

CSS allows animation of HTML elements without using JavaScript.To use CSS animation, you must first specify some keyframes for the animation.`@Keyframes` hold what styles the element will have at certain times.
__For example:__
```css
div {

    animation: example 5s linear 2s infinite alternate;
    /*
    animation-name: example;
    animation-duration: 5s;
    animation-timing-function: linear;
    animation-delay: 2s;
    animation-iteration-count: infinite;
    animation-direction: alternate;
    */
}

@keyframes example {

  0%   {background-color:red;}
  25%  {background-color:yellow;}
  50%  {background-color:blue;}
  75%  {background-color:green;}
  100% {background-color:red;}

}
```

The `animation-name` property specifies the name for the animation which is used for calling later while keyframing.


The `animation-duration` property defines how long time an animation should take to complete.


The `animation-timing-function` property specifies the speed curve of the animation.The `animation-timing-function` property can have the following values:

- ease - Specifies an animation with a slow start, then fast, then end slowly (this is default)
- linear - Specifies an animation with the same speed from start to end
- ease-in - Specifies an animation with a slow start
- ease-out - Specifies an animation with a slow end
- ease-in-out - Specifies an animation with a slow start and end
- cubic-bezier(n,n,n,n) - Lets you define your own values in a cubic-bezier function


The `animation-delay` property specifies a delay for the start of an animation.


The `animation-iteration-count` property specifies the number of times an animation should run.


The `animation-direction` property specifies whether an animation should be played forwards, backwards or in alternate cycles.The `animation-direction` property can have the following values:

- normal - The animation is played as normal (forwards). This is default
- reverse - The animation is played in reverse direction (backwards)
- alternate - The animation is played forwards first, then backwards
- alternate-reverse - The animation is played backwards first, then forwards
