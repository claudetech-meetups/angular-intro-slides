## Project creation

```sh
$ leaves new angular-blog
$ cd angular-blog
$ leaves install jquery angular angular-resource bootstrap angular-ui-router
```

Rename `assets/js/app.coffee` to `assets/js/app.js`,

erase `assets/css/main.styl` content and edit `views/layout.jade`.

```jade
// views/layout.jade
html
  head
    ....

    link(rel="stylesheet" href="components/bootstrap/dist/css/bootstrap.min.css")
    link(rel="stylesheet" href="components/bootstrap/dist/css/bootstrap-theme.min.css")

    script(src="components/jquery/dist/jquery.min.js")
    script(src="components/angular/angular.min.js")
    script(src="components/angular-resource/angular-resource.min.js")
    script(src="components/angular-ui-router/release/angular-ui-router.min.js")
    script(src="components/bootstrap/dist/js/bootstrap.min.js")

    script(src="js/app.js")
  body
    block content
```
