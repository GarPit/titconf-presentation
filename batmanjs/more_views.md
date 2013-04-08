!SLIDE title-and-content smbullets incremental

# More data-* attributes

* data-bind-attr

    ```html
    <img data-bind-src="post.imageURL"></img>
    ```

* data-event-click

    ```html
    <a data-event-click="controllers.Posts.buttonWasClicked"></a>
    ```

* data-event-change

    ```html
    <select data-event-change="controllers.Posts.selectChanged"></a>
    ```

* data-event-submit

    ```html
    <form data-event-submit="controllers.Posts.create">
    ...
    </form>
    ```

* data-partial

    ```html
    <div data-partial="sessions/new" />
    ```
