# Question Five
## An anagram of a word is just a rearrangement of its letters. How many different anagrams of “troublemakings” are there?

Because an anagram is just a rearrangement of all the letters in a word, in this case, we are arranging *n* distinct objects with the number of different arrangements (permutations) given by *n*!.

- The word "troublemakings" has 14 letters: T, R, O, U, B, L, E, M, A, K, I, N, G, S. All of these letters are distinct.

- **Permutation Formula:** Using the Permutation formula, we will set n and k to 14, getting P(n,k) because we are doing 14 permutations (k) of 14 elements (14). 
- By applying the formula: $\frac{n!}{(n-k)!}$ as $\frac{14!}{0!}$ giving us $14!$ because the factorial of zero is one. 
- With this we get: ``` 14! = 14 x 13 x 12 x ... x 1 ```

Giving us an answer of $8.717 \times 10^{10}$ or $87,178,291,200$
