!SLIDE title-and-content

# Bad Javascript

```javascript
$(document).ready(function(){
  ...
```
```javascript
$("select#country").on('change', function(){
  ...
```
```javascript
$.get("/cities",
    {
        country_id: $(this).val()
    },
    function(data){
        $("select#city").html(data);
        ...
    }
);
return false;
```

![burglar](../images/burglar.jpg)
![burglar2](../images/burglar2.jpg)
