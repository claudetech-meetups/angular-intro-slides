## Add links

[ui-router](https://github.com/angular-ui/ui-router) uses `ui-sref`
to make link instead of normal `href` or `ng-href` attributes.

```jade
// views/posts/index.jade
...
        a.small(ui-sref="show({ id: post.id })") See more
```
