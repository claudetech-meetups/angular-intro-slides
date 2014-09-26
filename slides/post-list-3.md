## Some solutions

* Use `ng-bind` instead of `{{}}`
* Use `date` filter
* We will see how to render markdown in content later on
* Use `limitTo` filter

```slim
.posts(ng-controller="PostIndexCtrl")
  .post.row
    .row
      .col-xs-12
        h2(ng-bind="post.title")
        small.date(ng-bind="post.date|date:'y/M/d'")
    .row.content
      .col-xs-12(ng-bind="post.content|limitTo:100")
    .row
      .col-xs-12
        a.small(href="#") See more
```
