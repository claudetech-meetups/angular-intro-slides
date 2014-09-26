## Filter query

Check if there is a category defined and adapt query.

```js
// assets/js/controllers/posts/index.js

angular.module('BlogApp').controller('PostIndexCtrl', [
  '$scope', '$stateParams', 'Post', function ($scope, $stateParams, Post) {
    var search = $stateParams.category ? {category_id: $stateParams.category} : {};
    Post.query(search, function (posts) {
      $scope.posts = posts;
    });
  }
]);
```
