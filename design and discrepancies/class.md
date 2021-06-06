https://github.com/ponylang/rfcs/issues/187
```pony
class Point
  var x: F64
  var y: F64

  new create(this.x, this.y)
```

```pony
class Point
  var x: F64
  var y: F64

  new create(var this.x: F64, var this.y: F64)
```
