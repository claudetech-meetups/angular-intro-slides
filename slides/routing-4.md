## Setup router

Controllers should be defined in routes.

```js
      .state('index', {
        url: '/',
        templateUrl: 'posts/index.html',
        controller: 'PostIndexCtrl'
      })
      .state('show', {
        url: '/posts/:id',
        templateUrl: 'posts/show.html',
        controller: 'PostShowCtrl'
      });
```

and removed from `views/posts/index.jade` and `views/posts/show.jade`.

```jade
// views/posts/show.jade
.post.row
  ...
```
