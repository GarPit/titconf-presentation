!SLIDE title-and-content bullets incremental

# Копаем глубже

```javascript
user.constructor == User
```

### user.prototype не то же самое, что User.prototype

```javascript
user.__proto__ == User.prototype
user.constructor.prototype == User.prototype
user.constructor.prototype == user.__proto__
```
