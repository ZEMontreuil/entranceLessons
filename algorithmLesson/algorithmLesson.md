# Algorithm Tracing #

**Algorithms** are sets of instructions that receieve some form of input, perform some sort of process using those inputs, and produce some sort of output.

Some very simple examples of Algorithms could be:

```
INPUT(A, B)
C = A + B
OUTPUT(C)
```

- Inputs `A = 1` and `B = 2` produce output `C = 3`
- Inputs `A = 100` and `B = -75` produce output `C = 25`

```
INPUT (I, J)
If (I = TRUE & J = TRUE then K = TRUE)
OUTPUT(K)
```
- Inputs `I = TRUE` and `J = TRUE` produce output `K = TRUE`
- Inputs `I = FALSE` and `J = TRUE` produce output `K = FALSE`

```
INPUT (X)
WHILE X >= 0
{
  X = X - Y
  OUTPUT X
}
```
- If input `X = 6` and `Y = 2`  output is `X = 6, X = 4, X = 2, X = 0`
- If input `X = 0` and `Y = 5` then output is `X = 0`

Algorithms are a fundamental part of computer programming, and one of the main advantages that a computer has is the ability to repeatedly process algorithms many times, much faster than humans.

## Algorithm Tracing ##
Although the majority of algorithms are performed by computers, they are typically written by humans. 

Being a succesful programmer often comes down to being able to **trace an algorithm**: following the values of inputs or other values as they pass through algorithms, in order to predict their final output.

For example, what output do we expect from this algorithm: 

```
INPUT (X, Y)
IF (X > Y) THEN X = X - Y
ELSE X = X + Y

IF (Y > X) 
OUTPUT(TRUE)
ELSE
OUTPUT(FALSE)
```
. . . if our inputs are X = 5 and Y = 7?

1. `IF (X > Y) THEN X = X - Y`
Since x is not greater than Y, we skip this step to:

2. `ELSE X = X + Y`
So X becomes X + Y, which is 5 + 7; X = 12.

3. `IF (Y > X) OUTPUT(TRUE)`
Since X is now 12, and Y (7) is not greater than 12, we skip this step.

4. `ELSE OUTPUT(FALSE)`
We reach the final component of our algorithm: our output is `FALSE`.
