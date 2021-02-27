# CPython

This is my fork of CPython just for fun.

So far differences are only syntactic

Here are some examples of some things that look different

```python
def sqrt(a):
  from math import sqrt as _sqrt
  if a < 0:
    yeet ValueError('sqrt of negative number')
  return _sqrt(a)

lst = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
lst = list(filter({ x => x % 2 == 0}, lst))
lst = list(map({ x => x ** 2 }, lst))
print(lst)
```

`raise` is now `yeet`

`lambda : <expr>` is now `{ => <expr> }`

`lambda x, y, z: <expr>` is now `{ x, y, z => x + y * z }`

