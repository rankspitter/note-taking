
Cryptosystems like RSA works on numbers, but messages are made up of characters. How should we convert our messages into numbers so that mathematical operations can be applied?  
  
The most common way is to take the ordinal bytes of the message, convert them into hexadecimal, and concatenate. This can be interpreted as a base-16/hexadecimal number, and also represented in base-10/decimal.



### Challenge 

Convert the following integer back into a message:


### Solved

```python
from Crypto.Util.number import *
long_number = 11515195063862318899931685488813747395775516287289682636499965282714637259206269
flag  = long_to_bytes(long_number)
print(flag)

```


### Description

converts the large integer `long_number` into a byte string using the `long_to_bytes()` function provided by the `Crypto.Util.number` module.



### Flag:

```
crypto{3nc0d1n6_4ll_7h3_w4y_d0wn}
```