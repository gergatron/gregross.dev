---
title: 'Animation'
order: 7
showToc: true
---

## 2d Transforms 

- translate() to move elements around
- rotate() to rotate elements
- scale() to scale elements in size
- skew() to twist or slant an element
- matrix() a way to perform any of the above operations using a matrix of 6 elements, a less user friendly syntax but less verbose

### We also have axis-specific functions:

- translateX() to move elements around on the X axis
- translateY() to move elements around on the Y axis
- scaleX() to scale elements in size on the X axis
- scaleY() to scale elements in size on the Y axis
- skewX() to twist or slant an element on the X axis
- skewY() to twist or slant an element on the Y axis

## 3d Transforms 

- translateZ()
- otateZ()
- scaleZ()


## TRANSITIONS
```scss
transition: property
            duration
            timing-function
            delay;
```

### transition-timing-function

- linear
- ease
- ease-in
- ease-out
- ease-in-out

https://flavio-css-transitions-easings.glitch.me/

## Animations 

```scss
  animation: name
             duration
             timing-function
             delay
             iteration-count
             direction
             fill-mode
             play-state;
```
#
```scss
.container {
  animation: spin 10s linear infinite;
}
```
#
```scss
  @keyframes spin {
    0% {
      transform: rotateZ(0);
    }
    100% {
      transform: rotateZ(360deg);
    }
  }
```

https://flavio-css-animations-tutorial.glitch.me/


## JavaScript events for CSS Animations

- animationstart
- animationend
- animationiteration