# Big-O Deep Dive Quiz (Interactive)

Score yourself: 2 points each (20 total).

## Section A — Multiple Choice

1. Which is true for Python list `append`?
   - A) Always `O(n)`
   - B) Amortized `O(1)`
   - C) Worst-case `O(1)` only
   - D) `O(log n)`

2. Which operation is most likely `O(n)` on dynamic arrays?
   - A) Access by index
   - B) Append at end
   - C) Insert at front
   - D) Pop at end

3. If algorithm A is `O(n)` time and `O(n)` space, B is `O(n log n)` time and `O(1)` space, which is always better?
   - A) A always
   - B) B always
   - C) Depends on constraints
   - D) Neither can be implemented

4. `for x in a: if x in list_b:` where both are lists gives typical complexity:
   - A) `O(n+m)`
   - B) `O(n log m)`
   - C) `O(nm)`
   - D) `O(log n)`

5. Big-O hides:
   - A) growth class only
   - B) constants and low-order terms
   - C) machine-level effects
   - D) all of the above

## Section B — Short Answer

6. Why can in-place algorithms still use more than `O(1)` total memory sometimes?
7. Give one example where extra space is preferred for correctness or maintainability.
8. Explain auxiliary space vs total space in one paragraph.
9. Analyze this quickly: two separate loops over `n` then sort -> complexity?
10. Give a production reason to avoid mutating input in-place.

---

## Answer Key

1-B, 2-C, 3-C, 4-C, 5-D

Suggested points for short answers:
- Q6 recursion stack mention
- Q7 stable behavior/readability/non-mutating requirement
- Q8 excludes input vs includes all allocations
- Q9 `O(n + n + n log n) = O(n log n)`
- Q10 immutability contracts, debugging, side effects
