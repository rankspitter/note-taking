
ASCII ?

is a 7 bit encoding standard which allows the representation using the integers 0-127.


[ASCII TABLE ](https://upload.wikimedia.org/wikipedia/commons/thumb/1/1b/ASCII-Table-wide.svg/1280px-ASCII-Table-wide.svg.png)

# challenge

Using the below integer array, convert the numbers to their corresponding ASCII characters to obtain a flag.

```
[99, 114, 121, 112, 116, 111, 123, 65, 83, 67, 73, 73, 95, 112, 114, 49, 110, 116, 52, 98, 108, 51, 125]
```


solved 

```python
array = [99, 114, 121, 112, 116, 111, 123, 65, 83, 67, 73, 73, 95, 112, 114, 49, 110, 116, 52, 98, 108, 51, 125]

print(''.join([chr(i) for i in array]))
```

description:

```
use list comprehesion `[chr(i) for i in array]` iterates over each integer in the `array` and converts it into its corresponding ASCII character using the `chr()` function.
```


Flag :

```
crypto{ASCII_pr1nt4bl3}
```