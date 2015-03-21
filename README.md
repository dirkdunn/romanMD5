# romanMD5
A super cool encryption which uses ROT13 and MD5 to extra encrypt your data with roman swag.
![RomanMD5](http://dirkdunn.com/rot13.png "RomanMD5")

When called with just a string to encrpyt, RomanMD5 returns your encrypted string, and a key.

```javascript
var romanMD5 = require("./romanMD5");
romanMD5("String to encrypt.") /* => [ '9s576311r04964777191ro464srs4q20', 587 ] */
```

If you want to retrieve the same encryption for that particular string again, simply call the function
again with the key value as the second parameter.

```javascript
romanMD5("String to encrypt.",587) /* => [ '9s576311r04964777191ro464srs4q20', 587 ] */
```

That's it, you can also get RomanMD5 on npm.

```
npm install romanmd5
```

Enjoy! and feel free to make a pull request.