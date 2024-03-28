
Modern cryptography with XOR operation

**Challenge code** 
```python
ords = [81, 64, 75, 66, 70, 93, 73, 72, 1, 92, 109, 2, 84, 109, 66, 75, 70, 90, 2, 92, 79]

print("Here is your flag:")
print("".join(chr(o ^ 0x32) for o in ords))

```

this python code have a list of integers called `ords` and applies the hexadecimal value `0x32` to each integer in the list by a bitwise XOR operation(^). Next, it uses the chr() function and joins them into a single string using the join() function.


Let's break down the expression `81 ^ 0x32 `, where `0x32 = 50`
the bitwise XOR operation step by step:
- `81` in binary is `1010001`.
- `50` in binary is `110010`.

``` scss
   1010001   (81)
^  0110010   (50)
__________
   1100011   (99)

```

So, `81 ^ 50` equals `99` ,represented by the character `c`

Flag :
```
crypto{z3n_0f_pyth0n}
```

