# QR code generator Javascript ES6 module

# A spiritual fork of QRious - qrious es6
I needed es6 modules compatible version of the project QRious.

I didn't fork the actual qrious repo, but without any bad intentions. I just didn't want to copy all files related to project. 

Check the actual repository:
https://github.com/neocotic/qrious

Also, maybe do not depend on this repo for an always up-to-date es6 version of qrious.

If you inspect my modification to neocotic's original code, you will see I did some very basic edits to make it into es6.

So, for future versions of qrious, you can take neocotic's latest code and edit to make it es6.

(that said, the last update was 5 years ago in 2017, so maybe this is recent enough for you)

# How to generate QR codes?

In your code, simply 

```javascript
import { QRious } from "qrious.js";

const qr = new QRious(/* could define initial settings here*/); 

qr.value = "cats are cool";

console.log(qr.toDataURL());
```

Then refer to https://github.com/neocotic/qrious/tree/master#readme


In the original repo, they mention a global "QRious" object. Here we just import it from the module, but it is identical to the global one. 

# Installation

You can either download this `qrious.js` file to your project and import from that static copy, or import from jsdelivr.

Here is the format if you want jsdelivr:

```javascript

import { QRious } from "https://cdn.jsdelivr.net/gh/sorcererinferior/qrious-es6@main/qrious.js"

```

