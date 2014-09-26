## Create basic layout

Add header to `views/layout.jade`

```
html
  head
    ....
  body(ng-app="")
    .container
      nav.navbar.navbar-default
        .container-fluid
          .navbar-header
            a.navbar-brand(href="#") Blog
      .row
        .col-xs-8
          block content
        .col-xs-4
          h3 Categories
            ul.list-unstyled
              li: a.small(href="#") Plenty of categories
          h3 Admin
            ul.list-unstyled
              li: a.small(href="#") Add post
```
