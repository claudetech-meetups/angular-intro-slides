## Fetch single post

Use `$stateParams` to get id, and get post from server.

```js
// assets/js/controllers/posts/show.js
angular.module('BlogApp').controller('PostShowCtrl', [
  '$scope', '$stateParams', 'Post', function ($scope, $stateParams, Post) {
    Post.get({id: $stateParams.id}, function (post) {
      $scope.post = post;
    });
  }
]);
```
