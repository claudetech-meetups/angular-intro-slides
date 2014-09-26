## Create categories controller

As for posts, query to get all the categories.

```js
angular.module('BlogApp').controller('CategoryIndexCtrl', [
  '$scope', 'Category', function ($scope, Category) {
    Category.query(function (categories) {
      $scope.categories = categories;
    });
  }
]);
```
