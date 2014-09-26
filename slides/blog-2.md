## Create basic layout

Create empty `views/_post_list.jade` and edit `views/index.jade`.

```slim
// views/index.jade
extends ./layout.jade

block content
  nav.navbar.navbar-default
    .container-fluid
      .navbar-header
        a.navbar-brand(href="#") Blog

  .row
    .col-xs-8
      h3 Posts
        include ./_post_list
    .col-xs-4
      h3 Categories
```
