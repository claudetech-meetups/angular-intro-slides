## Use API

Add `ngResource` module as a dependency.

```js
// assets/js/app.js
angular.module('BlogApp', [
  'ui.router',
  'ngResource'
]);
...
```

Try it

```js
// assets/js/controllers/posts/index.js
angular.module('BlogApp').controller('PostShowCtrl', [
  '$scope', '$resource', function ($scope, $resource) {
    ...
    var Post = $resource('http://angular-tutorial-api.herokuapp.com/posts/:id');
    Post.query(function (posts) {
      console.log(posts[0]);
      $scope.posts = posts;
    });
  }
]);
```
