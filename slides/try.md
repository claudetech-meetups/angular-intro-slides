## Try AngularJS

Initialize application

```jade
// views/layout.jade
html
  head
    ...
  body(ng-app="")
    block content
```

Try two-way data binding:

Output variable value with: `{{variable}}`.

Change variable value with: `ng-model="variable"`

```jade
// views/index.jade
extends ./layout.jade

block content
  input(ng-model="variable")
  span {{variable}}
```
