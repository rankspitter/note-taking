
Hexadecimal can be used in such a way to represent ASCII strings. First each letter is converted to an ordinal number according to the ASCII table . Then the decimal numbers are converted to base-16 numbers, otherwise known as hexadecimal. The numbers can be combined together, into one long hex string.


# challenge

Included below is a flag encoded as a hex string. Decode this back into bytes to get the flag.

``` scss
63727970746f7b596f755f77696c6c5f62655f776f726b696e675f776974685f6865785f737472696e67735f615f6c6f747d
```

```python
hex_flag = '63727970746f7b596f755f77696c6c5f62655f776f726b696e675f776974685f6865785f737472696e67735f615f6c6f747d'

flag = bytes.fromhex(hex_flag)

print(flag)
```

description :
use `bytes.fromhex()` can be used to convert hex to bytes.