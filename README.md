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
