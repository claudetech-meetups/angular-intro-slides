## Show categories

Create partial

```jade
// views/categories/index.jade

.block.categories(ng-controller="CategoryIndexCtrl")
  h3 Categories
  ul.list-unstyled
    li(ng-repeat="category in categories")
      a.small(ui-sref="index({category: category.id})" ng-bind="category.name")
```

Change layout to use partial.

``` views/layout.jade
....
        .col-xs-4
          include ./categories/index
          .block.admin
            h3 Admin
              ul.list-unstyled
                li: a.small(ui-sref="new") Add post

```
