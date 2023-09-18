# learningAPL
## Leetcode exercises

### [1. Two Sum](https://leetcode.com/problems/two-sum/)
````APL
solution1 ← {1-⍨⊃⍸(∘.≠⍨⍳≢⍵)∧⍺=∘.+⍨⍵}    ⍝ base 0 index
solution2 ← {⊃⍸(∘.≠⍨⍳≢⍵)∧⍺=∘.+⍨⍵}       ⍝ base 1 index
````
The solutions however, are  $O(n^2)$.

### [9. Palindrome Number](https://leetcode.com/problems/palindrome-number/)
````APL
solution ← (⌽≡⊢)⍕∘⊢    ⍝ point free solution
````

### [136. Single Number](https://leetcode.com/problems/single-number/)
````APL
solution1 ← {⍵~⍵/⍨~≠⍵}
````
The solution is not $O(n)$.
````APL
solution2 ← 2⊥≠/2⊥⍣¯1⊢e
````
This solution uses xor to filter the binary representation of every number.
