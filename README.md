# webgl-security
public key encryption + arbitrary precision (max modulo word size 128 bit?, vec4?) using webgl etc. e.g. RSA, ECC, Lattice...


Currently just a cute idea I have in my head, no code committed yet.

Although I have some ideas, where to start.

It will be DH-ish algorithms first.

Key exchange, Signing, Confirmation, and then maybe some symmetric ones e.g. Blowfish.
Also, why reinvent the wheel when you have emscripten.

WiP.

Ask "stupid" questions like:
* Can big integer scalar operations be expressed as matrix transformations? [Because we can use these libraries.](http://blog.tojicode.com/2010/06/stupidly-fast-webgl-matricies.html)
* 4x4, word-size 128 bit, is the maximum precision?
* What is precision? vec4 is [double, double, double, double]?

Or...

Find an openGL mathlib with arbitrary-prec. (opt. OpenGL 2.0 ES, for mobile?), but transpileable via Emscripten, then profit?!

Or...

* Read [this](http://www.html5rocks.com/en/tutorials/webgl/webgl_fundamentals/)
* Read [this](https://www.khronos.org/registry/webgl/specs/1.0/#5.14.5)
* Rewrite [this](http://www.bealto.com/mp-mandelbrot_fp128-opencl.html) in webGL from openCL.
