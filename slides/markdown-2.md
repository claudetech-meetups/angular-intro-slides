## Display formatted markdown

We use `ng-bind-html` to display HTML and not escaped values.

```jade
.post.row
  ....
  .row.content
    .col-xs-12(ng-bind-html="post.content|markdown")
```
