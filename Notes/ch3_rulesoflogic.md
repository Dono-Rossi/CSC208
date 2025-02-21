# Rules of Logic

## Notes
- **Truth Tables**
	- Truth tables are used to explore the relationships between different logical statements.
	- They help determine whether statements are logically equivalent.
	- A truth table lists all possible combinations of truth values for a set of statements and their resulting truth values.
- **Logical Equivalence**
	- Two statements are logically equivalent if they have the same truth values in all possible scenarios.
	- Logical equivalence allows us to simplify complex logical statements.
- **Deduction Rules**
	- Deduction rules are used to derive conclusions from premises in a logically valid manner.
	- Examples include Modus Ponens (if 𝑃 → 𝑄 and 𝑃 are true, then 𝑄 must be true) and Modus Tollens (if 𝑃 → 𝑄 and ¬𝑄 are true, then ¬𝑃 must be true).

## Questions from Blu's list

### 1.3.2
#### Make a truth table for the statement ~P $\lor$ Q
|  p  |  q  |  ~p or q  |
|-----|-----|-----------|
|  1  |  1  |     1     |
|  1  |  0  |     0     |
|  0  |  1  |     1     |
|  0  |  0  |     1     |

---

### 1.3.3
#### Analyze the statement, “If you get more doubles than any other player, then you will lose, or if you lose, then you must have bought the most properties,” using truth tables.

|  d  |  l  |  p  |  d => l  |  l => p  |  (d => l) or (l => p)  |
|-----|-----|-----|----------|----------|------------------------|
|  1  |  1  |  1  |    1     |    1     |           1            |
|  1  |  1  |  0  |    1     |    0     |           1            |
|  1  |  0  |  1  |    0     |    1     |           1            |
|  1  |  0  |  0  |    0     |    1     |           1            |
|  0  |  1  |  1  |    1     |    1     |           1            |
|  0  |  1  |  0  |    1     |    0     |           1            |
|  0  |  0  |  1  |    1     |    1     |           1            |
|  0  |  0  |  0  |    1     |    1     |           1            |

(D → L) ⋁ (L → P) Where D is if you get more doubles than any other player, L is you will lose, and P means you bought the most properties.

---

### 1.3.6
#### Are the statements, “It will not rain or snow,” and, “It will not rain and it will not snow,” logically equivalent?

|  r  |  s  |  ~(r or s)  |  ~r and ~s  |
|-----|-----|-------------|-------------|
|  1  |  1  |      0      |      0      |
|  1  |  0  |      0      |      0      |
|  0  |  1  |      0      |      0      |
|  0  |  0  |      1      |      1      |

Yes, the two statements are logically equivalent due to De Morgan's Law.

---

### 1.3.8
#### Prove that the statements ~(P => Q) and P $\land$ ~Q are logically equivalent without using truth tables.

As implications are disjunctions, ~(P => Q) is equal to ~(~P $\lor$ Q). Now, using DeMorgan's law, the negation of a disjuntion is logially equivalent to conjunction of negation, turning the disjunction into ~~P $\land$ ~Q. The negatives infront of the P to give P $\land$ ~Q.

---

### 1.3.10
Are the statements (P $\lor$ Q) => R and (P => R) $\lor$ (Q => R) logically equivalent?

|  p  |  q  |  r  |  (p or q) => r  |  (p => r) or (q => r)  |
|-----|-----|-----|-----------------|------------------------|
|  1  |  1  |  1  |        1        |           1            |
|  1  |  1  |  0  |        0        |           0            |
|  1  |  0  |  1  |        1        |           1            |
|  1  |  0  |  0  |        0        |           1            |
|  0  |  1  |  1  |        1        |           1            |
|  0  |  1  |  0  |        0        |           1            |
|  0  |  0  |  1  |        1        |           1            |
|  0  |  0  |  0  |        1        |           1            |

By looking at rows four and six it can be deduced that these statements are not logically equivalent.

---

### 1.3.14
#### Show that the following is a valid deduction rule.
 p => q<br>
~p => q<br>
\--------<br>
$\therefore$ q

|  p  |  q  |  ~p  |  p  => q  |  ~p => q  |
|-----|-----|------|-----------|-----------|
|  1  |  1  |  1   |     1     |     1     |
|  1  |  1  |  0   |     1     |     1     |
|  1  |  0  |  1   |     0     |     0     |
|  1  |  0  |  0   |     0     |     1     |
|  0  |  1  |  1   |     1     |     1     |
|  0  |  1  |  0   |     1     |     1     |
|  0  |  0  |  1   |     1     |     0     |
|  0  |  0  |  0   |     1     |     1     |

q is true in the same rows that (p => q) and (~p => q) are true therefore it's a valid deduction.

---

### 1.3.15
#### Decide whether the following is a valid deduction rule. <br>
p => r <br>
q => r <br>
  r <br>
\----<br>

$\therefore$ Q $\lor$ Q

|  p  |  q  |  r  |  p  => q  |  q => r  |  p or q  |
|-----|-----|-----|-----------|----------|----------|
|  1  |  1  |  1  |     1     |    1     |    1     |
|  1  |  1  |  0  |     1     |    0     |    1     |
|  1  |  0  |  1  |     0     |    1     |    1     |
|  1  |  0  |  0  |     0     |    1     |    1     |
|  0  |  1  |  1  |     1     |    1     |    1     |
|  0  |  1  |  0  |     1     |    0     |    1     |
|  0  |  0  |  1  |     1     |    1     |    0     |
|  0  |  0  |  0  |     1     |    1     |    0     |

On the second-to-last row, all three premises of the argument are true, but the conclusion is false. Therefore, this is not a valid deduction rule.
