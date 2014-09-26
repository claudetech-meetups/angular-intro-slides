## Create basic layout

Create empty `views/posts/index.jade` and edit `views/index.jade`.

```slim
// views/index.jade
extends ./layout.jade

block content
  include ./posts/index
```
