## Make it a list

Add dummy data in the controller.

```js
function PostIndexCtrl($scope) {
  $scope.posts = [{
    title: "Post title",
    content: "Post content",
    date: new Date()
  }, {
    title: "Post title 2",
    content: "Post content 2",
    date: new Date()
  }];
}
```

Use `ng-repeat`

```slim
.posts(ng-controller="PostIndexCtrl")
  .post.row(ng-repeat="post in posts")
    ...
```
