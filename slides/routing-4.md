## Setup router

Controllers should be defined in routes.

```js
      .state('index', {
        url: '/',
        templateUrl: 'post_index.html',
        controller: 'PostIndexCtrl'
      })
      .state('show', {
        url: '/posts/:id',
        templateUrl: 'post_show.html',
        controller: 'PostShowCtrl'
      });
```

and removed from `views/post_index.jade` and `views/post_show.jade`.

```jade
// views/post_show.jade
.post.row
  ...
```
