!SLIDE title-and-content

# Batman.Controller

```coffeescript
# контроллеры - синглтон классы с маршрутизированными методами-экшенами
# т.к. синглтоны, переменные экземпляра существуют пока запущено приложение
class PostsController extends Batman.Controller
  index: ->
    Post.load (error, posts) =>
      throw error if error
      @set 'posts', posts
    # implicit @render

  show: (params) ->
    Post.find params['id'], (error, post) =>
      throw error if error
      @set 'post', post

  buttonWasClicked: (node, event) ->
    $(node).toggleClass('activated')
    @redirect Post # redirects to "/posts"
```
