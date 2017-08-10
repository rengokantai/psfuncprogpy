# psfuncprogpy

## 7. Recursion
### 2 Demo: Summing, Recursively
```
def s(n):
  if n == 0:
    return n
  else:
    return n + a(n-1)

print(s(1000))
import sys
print(sys.getrecursionlimit())
```

### 4 Demo: Tail Recursive Sum  Function
```
def s(n,acc=0):
  if n==0:
    return acc
  else:
     return s(n-1,acc+n)

print(s(10))
```



### 6 Demo: Fibonacci,Trampoline Style
```
import types
def tramp(gen, *args, **kwargs):
  g = gen(*args, **kwargs)
  while isinstance(g,types.GeneratorType):
    g = next(g)
  return g
```


```
def f(n, curr=0,next=1):
  if n==0:
    return curr
  else:
    return f(n-1,next,curr+next)
print ([f(i) for i in range(10)])
```
