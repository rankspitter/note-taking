
another common encoding scheme is Base64, which allow us to represent binary data as an ASCII string using an alphabet of 64 characters. 

[How base64 encode](https://www.redhat.com/sysadmin/base64-encoding)


### Challenge

Take the below hex string, _decode_ it into bytes and then _encode_ it into Base64.

```scss
72bca9b68fc16ac7beeb8f849dca1d8a783e8acf9679bf9269f7bf
```

### Solved

```python
import base64

flag = '72bca9b68fc16ac7beeb8f849dca1d8a783e8acf9679bf9269f7bf'
flag = bytes.fromhex(flag)

print(base64.b64encode(flag)))
```

### Description:

This code converts a hexadecimal string (`hex_string`) into bytes using `bytes.fromhex()`, then encodes the bytes data to Base64 format using `base64.b64encode()`, and finally prints the Base64 encoded data after decoding it to a string.


### Flag: 

```
crypto/Base+64+Encoding+is+Web+Safe/
```