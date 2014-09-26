## Angular modules

Angular has native modules.
Declare `BlogApp` module with no depencies.

```js
// assets/js/app.js
angular.module('BlogApp', []);
```

Declare controllers as part of the module.

```js
// assets/js/controllers/posts/index.js
angular.module('BlogApp').controller('PostIndexCtrl', [
  '$scope', function ($scope) {
    ...
  }
]);
```

Same goes for `PostShowCtrl`.
