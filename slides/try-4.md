## Try AngularJS

React to events:

```jade
// views/index.jade
div(ng-controller="TestCtrl")
    span {{variable}}
    button(ng-click="action()")
```

```javascript
// assets/js/app.js
function TestCtrl($scope) {
  $scope.variable = "my variable text";
  $scope.action = function () {
    $scope.variable = "I just clicked!";
  };
}
```
