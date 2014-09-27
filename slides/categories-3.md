## Update routes

Update index routes to take `category` query parameter.

```
// assets/js/app.js
...

   $stateProvider
      .state('index', {
        url: '/?category',
        templateUrl: 'posts/index.html',
        controller: 'PostIndexCtrl'
      })
```

This is needed to pass `category` to `ui-sref` and
to read it from `$stateParams`.
