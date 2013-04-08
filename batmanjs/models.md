!SLIDE title-and-content

# Batman.Model

```coffeescript
class Post extends Batman.Model
    @encode 'title', 'content'
    ...

    @validate 'title', presence: yes, maxLength: 100
    @validate 'content', presence: yes, lengthWithin: [8,1024]
    ...

    @persist Batman.LocalStorage   # browser's localStorage
    # @persist Batman.RestStorage  # REST backend
    # @persist Batman.RailsStorage # Rails REST backend
    # @url = "/admin/products"
    # url: -> "/admin/products/#{@get('id')}"
    # urlPrefix: -> "http://api.mydomain.com"
    # @urlPrefix = "http://api.mydomain.com"
```
