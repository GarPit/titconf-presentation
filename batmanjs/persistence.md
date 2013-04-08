!SLIDE title-and-content

# Persistence

```coffeescript
# Работа со свойствами модели
post = new Post title: "TITConf"
post.get 'title' # TITConf
post.set 'title', "Welcome to TITConf"
```

```coffeescript
# Сохранение
post.save (error, record) ->
  throw error if error
  ...
```

```coffeescript
# Загрузка
Post.load (error, posts) ->
  throw error if error
  ...
Post.find 1, (error, post) ->
  # got error or post
```
