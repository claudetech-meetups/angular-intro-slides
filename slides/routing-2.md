## Setup view

First, add the view where to display the content of the route.

```jade
// views/index.jade
extends ./layout.jade

block content
  div(ui-view)
```
