## README audit vs `factorial.py`

### Title and summary

| Claim | Verdict | Evidence |
|---|---|---|
| “Beginner Python: Factorial” | **Supported** (as a label) | The file is a short Python script that computes a factorial. “Beginner” is framing, not a coded feature. |
| “A small Python program that calculates the factorial of a number using a `for` loop.” | **Supported** | `for i in range(1,n+1):` then `fact=fact*i`. |

### What the program does

| Claim | Verdict | Evidence |
|---|---|---|
| “`factorial.py` computes the factorial of `n`, where `n` is set to `5` in the code.” | **Supported** | `n=5` |
| “Starts with `fact = 1`” | **Supported** | `fact=1` |
| “Multiplies `fact` by each integer from `1` through `n`” | **Supported** | `range(1,n+1)` and `fact=fact*i` |
| “Prints the result” | **Supported** | `print(fact)` |
| Running as written prints `120` | **Supported** | With `n=5`, the loop is `1*2*3*4*5`, which is `120`. |
| “That is `5!` (`1 × 2 × 3 × 4 × 5`).” | **Supported** | Same loop with `n=5`. |
| “To calculate the factorial of a different number, change the value of `n` in the file.” | **Supported** | `n` is a variable used as the loop bound; there is no other input path. |
| “This program does not take keyboard input” | **Supported** | No `input()` (or similar). |
| “does not use extra libraries” | **Supported** | No `import` statements. |

### How to run it

| Claim | Verdict | Evidence |
|---|---|---|
| “Make sure Python is installed.” | **Not Supported** by the code | Environment requirement. The file is Python, but the source does not state that Python must be installed. |
| “Open a terminal in this folder.” | **Not Supported** by the code | Run-time instruction, not present in `factorial.py`. |
| Run with `python factorial.py` | **Not Supported** by the code | Standard way to launch the file, but the script itself does not document or encode this command. |

### Learning objective

| Claim | Verdict | Evidence |
|---|---|---|
| “Practice using a `for` loop and a running product to compute a factorial” | **Supported** (as a description of the code) | `for` loop plus `fact=fact*i`. |
| “a common beginner exercise in iteration and variables” | **Not Supported** by the code | Pedagogical opinion; nothing in the source asserts this. |

**Note:** The Colab notebook header in `factorial.py` is unused by the README and is not a README claim.