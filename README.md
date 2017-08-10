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

