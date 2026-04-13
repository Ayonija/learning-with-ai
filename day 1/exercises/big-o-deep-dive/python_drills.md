# Python Drills — Big-O Deep Dive

## Drill 1: Spot the Hidden Quadratic

```python
def build_front(n):
    a = []
    for i in range(n):
        a.insert(0, i)
    return a
```

1. Derive time complexity.
2. Rewrite to make it `O(n)`.

---

## Drill 2: Membership Optimization

```python
def count_hits(a, b):
    c = 0
    for x in a:
        if x in b:
            c += 1
    return c
```

Assume `len(a)=n`, `len(b)=m`.

Tasks:
- Analyze current complexity.
- Optimize using a better structure.
- Recompute time + extra space.

---

## Drill 3: Slicing Trap

```python
def pair_sum(a):
    s = 0
    while a:
        s += a[0] + a[-1]
        a = a[1:-1]
    return s
```

Tasks:
- Explain why this is slower than it appears.
- Give an in-place-index version.

---

## Drill 4: Interactive Reflection

For each of these methods, write a sticky-note explanation in one line:

- `append`
- `pop()`
- `pop(0)`
- `sort`
- slicing

Rule: explanation must include both time and memory impact.
