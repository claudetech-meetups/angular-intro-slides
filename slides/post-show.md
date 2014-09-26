## Show single post

Create `views/post_show.jade`, we will extend `layout.jade` for now.

```
extends ./layout.jade

block content
  .post.row(ng-controller="PostShowCtrl")
    .row
      .col-xs-12
        h2 {{post.title}}
        small.date {{post.date|date:'y/M/d'}}
    .row.content
      .col-xs-12 {{post.content}}
```

create `PostShowCtrl` function.

```js
// assets/js/app.js
....
function PostShowCtrl($scope) {
  $scope.post = {
    title: "Post title",
    content: "Post content",
    date: new Date()
  };
}
```

You can try to access your page: <a href="http://localhost:9000/post_show.html" target="_blank">localhost:9000/post_show.html</a>

