## Setup router

Configure to redirect to `/` when no route found,
and configure the routes.

```js
// assets/js/app.js

angular.module('BlogApp').config([
  '$stateProvider', '$urlRouterProvider', function ($stateProvider, $urlRouterProvider) {
    $urlRouterProvider.otherwise('/');

    $stateProvider
      .state('index', {
        url: '/',
        templateUrl: 'post_index.html'
      })
      .state('show', {
        url: '/posts/:id',
        templateUrl: 'post_show.html'
      });
  }
]);
```

Then, remove the `extends` and `block content` from `views/posts_show.jade`:
we don't need the whole layout.

You can now access your route:
<a href="http://localhost:9000/#/posts/1" target="_blank">localhost:9000/#/posts/1</a>
