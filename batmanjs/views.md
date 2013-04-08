!SLIDE title-and-content

# Batman.View

```html
<!-- index.html -->
<html>
  <body data-yield="main">
  </body>
</html>
```

```html
<!-- views/posts/index.html -->
<ul>
  <li data-foreach-post="posts" data-bind="post.title">
  </li>
</ul>
```

```html
<!-- views/posts/show.html -->
<h1 data-bind="post.title"></h1>
<p data-bind="post.content"></p>
```
