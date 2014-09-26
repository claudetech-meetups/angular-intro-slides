## Try AngularJS

Initialize variable:

```jade
// views/index.jade
extends ./layout.jade

block content
  div(ng-init="variable = 'plain text'")
    span {{variable}}
```

You can use any element, not just `div` and `span`.
