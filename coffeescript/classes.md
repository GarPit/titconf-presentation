!SLIDE title-and-content columns

# Классы и объекты

## Coffeescript

```coffeescript
class Animal
  constructor: (@name) ->

class Horse extends Animal
  move: ->
    alert "Galloping..."
```

## Javascript

```javascript
function Animal(name)
{
  this.name = name;
}

function Horse(name)
{
  Animal.call(this, name);
}

Horse.prototype = Object.create(Animal.prototype);
Horse.prototype.move = function()
{
  alert('Galloping...');
};
Horse.prototype.constructor = Horse;
```
