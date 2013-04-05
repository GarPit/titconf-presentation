!SLIDE title-and-content bullets incremental

# Прототипы

```javascript
function User() {
}
```

```javascript
User.prototype.greet = function() {
  return 'hello';
};
```

```javascript
var user = new User();
user.greet();
```
