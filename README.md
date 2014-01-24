typestring
==========
`typestring` is a simple JavaScript module providing an in-memory (string-in and
string-out) TypeScript compiler.

Installation
------------

    npm install typestring

Example
-------

    var ts = require('typestring');
    ts.compile('class Foo { public bar = 2; }');

Output string:

    var Foo = (function () {
        function Foo() {
            this.bar = 2;
        }
        return Foo;
    })();

License
-------
`typestring` is released under the terms of the
[MIT license](http://tldrlegal.com/license/mit-license). See **LICENSE**.
