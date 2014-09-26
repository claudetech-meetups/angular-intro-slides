## Make it a list

Add dummy data in the controller.

```js
function PostIndexCtrl($scope) {
  $scope.posts = [{
    id: 1,
    title: "Post title",
    content: "Post content",
    createdAt: new Date()
  }, {
    id: 2,
    title: "Post title 2",
    content: "Post content 2",
    createdAt: new Date()
  }];
}
```

Use `ng-repeat`

```slim
.posts(ng-controller="PostIndexCtrl")
  .post.row(ng-repeat="post in posts")
    ...
```
