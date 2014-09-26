## Create new post template

Bind the model created in the controller.

```jade
// views/posts/new.jade
h2 Create new post

form
  .form-group
    label(for="title") Title
    input#title.form-control(type="text" placeholder="Title" ng-model="post.title")
  .form-group
    label(for="content") Content
    textarea#content.form-control(rows="10" ng-model="post.content")
  .form-group
    select.form-control(ng-model="post.category_id")
  input.btn.btn-default(type="submit" value="Create")
```
