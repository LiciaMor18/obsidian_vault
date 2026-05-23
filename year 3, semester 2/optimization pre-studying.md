hopefully a little prep helps me out …..

## solve simplex method
we go with *dantzig’s rule* (biggest bite first)
and use *bland’s rule* only in case of a tie
remember we increase the function by $r_{\beta}\left( \frac{p_{\alpha}}{-q_{\alpha \beta}} \right)$
### edge cases
#### unboundedness
no negative coefficients when finding leaving basic variable. nothing gets smaller, you can shoot the entering variable to infinity. the functions is unbounded
- what about a feasible solution ? pg30

#### degenerancy
two or more equations give the exact smallest ratio when doing the ratio test. in this case, you *need* to use bland’s rule
	
What it means: Two basic variables hit 0 at the exact same time. You pick one to be the leaving variable. In your next dictionary, the other one will have a constant term of exactly 0 (e.g., s2​=0−2x2​+…).

The danger: A constant of 0 means in your next pivot, the minimum ratio will be 0. You will do a full pivot, but your Z value won't increase at all. 

#### multiple optimal solutions
one of the non-basic variables has a coefficient of 0 in the `z` row. this means we found the opt value, but we found another so
3. Multiple Optimal Solutions (The "Alternative Optima")

    How to spot it: You reach what looks like the final, optimal dictionary because there are no more positive coefficients in the Z equation. However, one of the non-basic variables has a coefficient of exactly 0 in the Z row.

    Example:
    Z=15−2x1​−0x2​−4s1​

    What it means: You have found the maximum profit (15). But because x2​ has a 0 coefficient, you could pivot x2​ into the basis without changing the Z value. This means the solution you found isn't the only solution. There is an entire line segment (or edge of the geometric shape) where every point yields that exact same maximum profit of 15.

4. Infeasibility (The "Bad Start")

    How to spot it: Before you even do your first pivot, one or more of the constant terms (the numbers standing alone) in your initial dictionary are negative.

    Example:
    s1​=−4−2x1​−x2​

    What it means: The standard Simplex method assumes that setting all non-basic variables to 0 gives you a valid, legal starting point (the origin). If doing so makes s1​=−4, you are violating the rule that all variables must be ≥0. You are starting outside the feasible region. To fix this, you cannot use the standard Simplex method; you have to use a special setup technique called the Two-Phase Method or the Big-M Method to mathematically "walk" into the valid region before you can start maximizing.