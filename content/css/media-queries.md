---
title: 'Media Queries'
order: 8
showToc: true
---

## Media Types

- all means all the media
- print used when printing
- screen used when the page is presented on a screen
- speech used for screen readers

## Media Queries
```scss
@media () {}
```
#
```scss 
@media screen and (max-width: 800px) and (min-width: 600px) and (orientation: landscape) {
  /* enter some CSS */
}
```

## Mobile First 
### Targets Larger Screens
```scss 
@media (min-width: 600px) {
  /* enter some CSS */
}
```