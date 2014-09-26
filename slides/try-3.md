## Try AngularJS

Use controller to initialize variable.

```slim
// views/index.jade
div(ng-controller="TestCtrl")
    span {{variable}}
```

Define controller in JS file.

`$scope` is injected by Angular on instanciation.


```javascript
// assets/js/app.js
function TestCtrl($scope) {
  $scope.variable = "my variable text";
}
```

Angular uses [DI](http://en.wikipedia.org/wiki/Dependency_injection) to instanciate controllers, services, etc.
