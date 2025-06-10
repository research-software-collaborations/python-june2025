# 003 - Fibonacci sequence

A sequence of numbers where the next element is the sum of the two previous. Often starting at 0,1 or 1,1.
```
It goes:
0, 1, 1, 2, 3, 5, 8, 13, 21, 34, 55, 89, 144, ....
```
The following implementation has an error. Do you see it? Fix the error and modify this code to reproduce 
the sequence above.

```python
def fibonacci(n):
    fib_seq = [0, 1]
    for i in range(0, n):
        fib_seq.append(fib_seq[i] + fib_seq[i-1])
    return fib_seq[:n]
print(fibonacci(10))
```