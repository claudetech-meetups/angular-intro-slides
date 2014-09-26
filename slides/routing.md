## Routing

Route in order to be able to have

* `/#/` -> all posts
* `/#/posts/:id` -> post with id = `:id`
* `/#/posts/new` -> new post

First, add [`ui.router`](https://github.com/angular-ui/ui-router) depency to the module.

```js
// assets/js/app.js
angular.module('BlogApp', [
  'ui.router'
]);
```
