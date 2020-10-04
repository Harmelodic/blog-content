Taken from [here](http://zerosixthree.se/vertical-align-anything-with-just-3-lines-of-css/)

It's a bit of CSS that will allow you to instantly vertically align a `<div>` within another `<div>`:

```css
.element {
    position: relative;
    top: 50%;
    transform: translateY(-50%);
}
```

Note: In Firefox, you may need to set the parent element's `height`.  
This was discovered when using this CSS on a child of `body` to position an element in the middle of the screen;

```css
body {
    height: 100%;
}
```
