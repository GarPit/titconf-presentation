!SLIDE title-and-content

# Ассоциации

```coffeescript
class Post extends Batman.Model
    @hasMany 'comments', options
    ...

class Comment extends Batman.Model
    @belongsTo 'post', options
    ...
    @encode 'content'
```

```coffeescript
post = new Post title: "TITConf", content: "OMG! Я на TITConf"
comment1 = new Comment content: "Мужык!"
comment2 = new Comment content: "О чем речь то?"

post.set 'comments', new Batman.Set(comment1, comment2)
```
