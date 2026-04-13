# Java Drills — Big-O Deep Dive

## Drill 1: ArrayList Cost Audit

```java
int f(ArrayList<Integer> list, int n) {
    for (int i = 0; i < n; i++) {
        list.add(0, i);
    }
    return list.size();
}
```

Tasks:
1. Complexity in terms of `n` and current list size.
2. Rewrite with better asymptotic behavior.

---

## Drill 2: Binary Search Upgrade

```java
int common(int[] a, int[] b) {
    int c = 0;
    for (int x : a) {
        for (int y : b) {
            if (x == y) c++;
        }
    }
    return c;
}
```

Tasks:
- Current time complexity?
- Improve with sorting + binary search.
- Optional: improve with hash set and compare space trade-off.

---

## Drill 3: Copy vs In-Place

You need to rotate an array right by `k`.

1. Design a copy-based solution and give complexity.
2. Design an in-place solution and give complexity.
3. Which would you ship for readability vs memory constraints?

---

## Drill 4: API Fluency Quickfire

For each method, write complexity and one caveat:

- `Arrays.sort`
- `Arrays.binarySearch`
- `Arrays.copyOf`
- `ArrayList.contains`
