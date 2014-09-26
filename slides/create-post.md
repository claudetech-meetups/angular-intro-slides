## New post controller

Create new JS file, and a fresh post to bind.

```js
// assets/js/controllers/posts/new.js
angular.module('BlogApp').controller('PostNewCtrl', [
  '$scope', 'Post', function ($scope, Post) {
    $scope.post = new Post();
  }
]);
```

and include it in `views/layout.jade`

```jade
script(src="js/controllers/posts/new.js")
```
