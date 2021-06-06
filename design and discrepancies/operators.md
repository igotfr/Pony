## Pipeline Operator
https://github.com/ponylang/rfcs/issues/89

https://github.com/ponylang/rfcs/issues/165
```pony
a |> f
// equivalent to
f(a)
```
```pony
b |2> f(a) // or b |1> f(a) if starting at 0
// equivalent to
f(a, b)
```
```pony
b |b_arg> f(a)
// equivalent to
f(a, where b_arg = b)
```
