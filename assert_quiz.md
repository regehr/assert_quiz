# Assert Quiz

For each of these assertions, determine whether it is good or
bad. Explain your reasoning.

If you need more background about assertions, consult the following sources.
- https://blog.regehr.org/archives/1091
- http://wiki.c2.com/?WhatAreAssertions
- http://pgbovine.net/programming-with-asserts.htm
- Chapter 2 of [Writing Solid Code](http://writingsolidcode.com/)

Here is an example of a very bad assertion:
  https://github.com/rohe/pysaml2/issues/451

1.
```
res = open(path, "r");
assert(res >= 0);
```

2.
```
assert(p = malloc(size));
```

3.
```
p = malloc(size);
assert(p);
```

4.
```
int array[length];
...
int index = hash_function(input);
assert(index >= 0 && index < length);
array[index] = -1;
```

5.
```
res = fclose(fd);
assert(res == 0);
```

6.
```
assert(tree_is_balanced(t));
```

7.
```
if (a == 42)
  doSomething();
else
  assert(false && "a should be 42");
otherCode();
```

8.
```
res = printf("%d\n", i);
assert(res > 0);
```

9.
```
if (func())
  x = 3;
else
  x = 17;
assert (x==3 || x==17);
```

10.
```
switch(x) {
case ...:
default:
   assert("unexpected value");
}
```

11.
```
assert(!"unreachable");
```

12.
```
assert(sizeof(some_struct) == 72);
```

13.
```
... calculate lengths of sides of a triangle ...
assert(short1 + short2 <= long + epsilon);
```

14.
```
std::map<int, int> map;
... code ...
assert(map[42] == 0);
... code ...
map.at(42) = 32;
```

15.
```
... calculate angles of a triangle ...
assert(angle1 + angle2 + angle3 - 180.0 < epsilon);
```

16.
```
assert(Index++ < Length);
```
