## Post list basic layout

Create sample content in `views/posts/index.jade`

```slim
// views/posts/index.jade
.post.row
  .row
    .col-xs-12
      h2 Title
      small.date 2014/09/12
  .row.content
    .col-xs-12
      p Quite
      p Long
      p Content
  .row
    .col-xs-12
      a.small(href="#") See more
```

Update style a little

```css
// assets/css/main.styl
.content
  margin-top 10px
  font-size 12pt
```
