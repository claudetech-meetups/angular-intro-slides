## Resolve categories

Better have categories before loading template.
Use custom made promise and resolve API result.


```js
// js/app.js
...
      .state('new', {
        url: '/posts/new',
        templateUrl: 'posts/new.html',
        controller: 'PostNewCtrl',
        resolve: {
          categories: ['$q', 'Category', function ($q, Category) {
            var deferred = $q.defer();
            Category.query(function (categories) {
              deferred.resolve(categories);
            });
            return deferred.promise;
          }]
        }
      })
      .state('show', {
        ....
```
