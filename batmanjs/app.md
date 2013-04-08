!SLIDE title-and-content

# Batman.App

```coffeescript
class Blog extends Batman.App
  @root 'posts#index'
  @route 'posts/special', 'posts#special'
  @resources 'posts'
  # @route 'posts', 'posts#index'
  # @route 'posts/new', 'posts#new'
  # @route 'posts/:id', 'posts#show'
  # @route 'posts/:id/edit', 'posts#edit'
  ...

window.Blog = Blog
$ ->
    Blog.run()
```
