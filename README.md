## Int64

Transform int64 between hex and dec(signed).

## Usage

```js
    var int64 = require('int64');
    var hex2dec = int64.hex2dec;
    var dec2hex = int64.dec2hex;
    console.log(hex2dec('1234567890abcdef'));
    console.log(dec2hex('-9223372036854775808'));

    // Example use with an 8-byte buffer:
    var buf = Buffer.from([ 250, 255, 255, 255, 255, 1, 2, 3 ]);
    console.log(buf.toString('hex')); // prints faffffffff010203
    console.log(hex2dec(buf.toString('hex'))); // prints -360287970206350845
```
