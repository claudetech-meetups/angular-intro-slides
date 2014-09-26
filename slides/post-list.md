## Build post list

Create controller in JS file:

```js
function PostIndexCtrl($scope) {
  $scope.post = {
    title: "Post title",
    content: "Post content",
    date: new Date()
  };
}
```

Wrap post list in a controller and use dummy data

```slim
.posts(ng-controller="PostIndexCtrl")
  .post.row
    .row
      .col-xs-12
        h2 {{post.title}}
        small.date {{post.date}}
    .row.content
      .col-xs-12 {{post.content}}
    .row
      .col-xs-12
        a.small(href="#") See more
```

and create the controller.
