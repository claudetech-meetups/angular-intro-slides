## Resolve categories

Use the categories resolved in the controller.

```js
// assets/js/controllers/posts/new.js


angular.module('BlogApp').controller('PostNewCtrl', [
  '$scope', 'Post', 'categories', function ($scope, Post, categories) {
    $scope.post = new Post();
    $scope.categories = categories;
  }
]);
```
