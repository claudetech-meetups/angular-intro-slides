## Create post

React to submit event

```jade
// views/posts/new.jade

form(ng-submit="createPost()")
```

Add handler for submit event.

```js
// js/controllers/posts/new.js
angular.module('BlogApp').controller('PostNewCtrl', [
  '$scope', 'Post', '$state', 'categories', function ($scope, Post, $state, categories) {
    ...
    $scope.createPost = function () {
      $scope.post.$save(function (post) {
        $state.go('index', {id: post.id});
      });
    };
    ...
```
