## Modularization

Let's start by splitting files.

```js
// assets/js/controllers/posts/index.js
function PostIndexCtrl($scope) {
    .....
}
```

```js
// assets/js/controllers/posts/show.js
function PostShowCtrl($scope) {
    .....
}
```

```jade
// views/layout.jade
html
  head
    ....
    script(src="js/app.js")
    script(src="js/controllers/posts/index.js")
    script(src="js/controllers/posts/show.js")
  body(ng-app="")
    ...
```
