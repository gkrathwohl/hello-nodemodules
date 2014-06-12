helloaddon
===

A node addon in C++ that is the functional equivalent of:

    module.exports.hello = function() { return 'world'; };

Building
---

To build:

* First run `$ node-gyp configure`. This gives us a build directory and a Makefile.
* Now run `$ node-gyp build` to actually build the `.node` bindings file. The file will be stored in `build/Release/`.

Testing
---

Take a look at `hello.js` and run $ node hello.js` to see an example of this module in action.

Node-Webkit Integration
---

To compile this module for node-webkit, run:

    $ nw-gyp rebuild --target=0.8.6
