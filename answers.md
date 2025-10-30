# CMPS 2200 Recitation 06
## Answers

**Name:** Davis Voelkel
**Name:** Isaiah Kushner


Place all written answers from `recitation-07.md` here for easier grading.



- **2)** The reccurence is W(n) =W(n-1) +W(n-2) +O(1) for updating the count and addition. This is clearly leaf dominated since we have two recursive calls, with alpha = 2. Because S(n) = S(n-1) + 0(1) $\in O(n)$ , there will be n levels and two additional recursive calls per recursive call. Therefore, W(n) $\in O(n^2)$.

- **3)** S(n) = max{S(n-1),S(n-2)} + O(1) = S(n-1) + O(n). Therefore we have n levels with 1 cost per level -> $S(n) \in O(n)$

- **4)** The counts: [34, 55, 34, 21, 13, 8, 5, 3, 2, 1, 1]. The pattern that emerges from right to left is that the counts follows the Fibbonacci Sequence. What is odd, however, is that n=0 is called the same amount as n=2 instead of 89 times as the pattern would suggest.

- **6)** Similar to the span of the recursive version, you only have to considering the work of W(n-1) since W(n-2) is included in W(n-1). Therefore, W(n)= W(n-1) + 1 $\in O(n).$

- **8)** Every index is computed once and called an additional 2 times at most. However, retrieval is O(1) so we only have to consider the computing of the F(i) which is two O(1) retrievals that happen n times from 1 to n. Therefore W(n) $\in O(n)$. Because this is purely iterative, the S(n) $\in O(n)$ as well.
