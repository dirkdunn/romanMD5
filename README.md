# romanMD5
Use your choice of ancient encryption plus MD5 to extra encrypt your data!
![RomanMD5](http://oi58.tinypic.com/ibfgp1.jpg "RomanMD5")

RomanMD5 runs a roman encryption of your choice, plus the MD5 encrpytion algorithm between a range of 100 and 1000 times. Each method will return an array of two items, the first item is the encrypted string, and the second is the key. The key is the number of times the string was encrypted with the roman encryption of choice and MD5. The library currently supports:

1. ROT13 Caesar Cipher
2. Polyalphanumeric Caesar Cipher


**Using Rot13**
```javascript
var romanMD5 = require("./romanmd5");
romanMD5.rot13Encrypt("String to encrypt.") /* => [ '9s576311r04964777191ro464srs4q20', 587 ] */
```

**Using Polyalphanumeric**
```javascript
var romanMD5 = require("./romanmd5");
romanMD5.polyAlphaEncrypt("Hello","snake") /* => [ 't3b57286lf800pg27e10w29mkx5d8k07', 819 ] */
```

If you want to retrieve the same encryption for that particular string again, simply call the function
again with all the previous parameters, plus the key value as the second parameter. 

**Rot13:**
```javascript
romanMD5.rot13Encrypt("String to encrypt.",587) /* =>  '9s576311r04964777191ro464srs4q20' */
```

**Polyalphanumeric:**
```javascript
romanMD5.polyAlphaEncrypt("Hello","snake",819) /* =>  't3b57286lf800pg27e10w29mkx5d8k07' */
```

That's it, you can also get RomanMD5 on npm.

```
npm install romanmd5
```

Feel free to extend the library with other old school encryptions and ciphers. Just be sure to follow the same pattern. Look forward to your pull requests. 