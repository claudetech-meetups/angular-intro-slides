## Create category factory

```js
// assets/js/resources/category.js
angular.module('BlogApp').factory('Category', [
  '$resource', function ($resource) {
    return $resource('http://angular-tutorial-api.herokuapp.com/categories/:id');
  }
]);
```

and add it to `layout.jade`
