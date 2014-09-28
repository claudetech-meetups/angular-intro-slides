## Format markdown

We are going to create a filter to format markdown.

```js
// assets/js/filters/markdown.js

angular.module('BlogApp').filter('markdown', [
  '$sce', function ($sce) {
    return function (input) {
      if (!input) {
        return '';
      }
      return $sce.trustAsHtml(markdown.toHTML(input));
    };
  }
]);
```

* `input` is the value to convert to markdown.
  We return empty string if undefined.
* The markdown is formatted in HTML, we need to trust the input
  to tell Angular it is safe.
* We suppose that the input is actually safe here,
  so some extra precautions would be needed when this is not the case.
