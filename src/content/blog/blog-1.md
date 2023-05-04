---
title: 'Basic CSS Reset'
description: 'Basic CSS reset to get a project started.'
author: 'Sunbear Day'
tags: ["css"]
---

```css
:is(*, *::before, *::after) {
  box-sizing: border-box;
}

* {
  margin: 0;
}

body {
  font-family: sans-serif;
  line-height: 1.5;
}

img, picture, video, canvas, svg {
  display: block;
  max-width: 100%;
}

:is(input, button, textarea, select) {
  font: inherit;
}

:is(p, h1, h2, h3, h4, h5, h6) {
  overflow-wrap: break-word;
}
```
