## Use `ng-options`

Dynamically show categories in `select` using `ng-options`.

```jade
form
  ...
  select.form-control(
    ng-model="post.category_id"
    ng-options="c.id as c.name for c in categories"
  )
```
