https://github.com/ponylang/rfcs/issues/188
```pony
cond
| 2 + 2 == 5 => "This will not be true"
| 2 * 2 == 3 => "Nor this"
| 1 + 1 == 2 => "But this will"
| true => "This is always true (equivalent to else)​"
end
```
```pony
match None
| if 2 + 2 == 5 => "This will not be true"
| if 2 * 2 == 3 => "Nor this"
| if 1 + 1 == 2 => "But this will"
| if true => "This is always true (equivalent to else)"
end
```
```pony
cond
  2 + 2 == 5 ->
    "This will not be true",
  2 * 2 == 3 ->
    "Nor this",
  1 + 1 == 2 ->
    "But this will",
  true ->
    "This is always true (equivalent to else)"
end
```
