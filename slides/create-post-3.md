## Add a new route

Careful, order matters!

```js
    $stateProvider
      .state('index', {
        .....
      })
      .state('new', {
        url: '/posts/new',
        templateUrl: 'posts/new.html',
        controller: 'PostNewCtrl'
      })
      .state('show', {
        .....
      });
```

And set link

```jade
// views/layout.jade
...
        .block.admin
          h3 Admin
            ul.list-unstyled
              li: a.small(ui-sref="new") Add post

```
