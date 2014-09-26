## Resource factory

We want to be able to use `Post` resource anywhere.

Let's make it a factory.

```js
// assets/js/resources/post.js
angular.module('BlogApp').factory('Post', [
  '$resource', function ($resource) {
    return $resource('http://angular-tutorial-api.herokuapp.com/posts/:id');
  }
]);
```

and include it in `views/layout.jade`

```jade
html
  head
    ...
    script(src="js/resources/post.js")
```
