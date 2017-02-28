# `Hello, World!`

Let's go through a TypeScript `Hello, World!` example.



# Get TypeScript Compiler

We have to set up a development environment locally.  If you prefer not
to do so, try [`Hello, World!` without Local Environment Setup][1].

[1]: hello-world-without-local-environment-setup.md

There are [a few ways][2] to get a TypeScript compiler.  For the purpose
of this tutorial, we will go with the simplest option: Node.js.

[2]: https://www.typescriptlang.org/index.html#download-links

1. Get Node.js from [https://nodejs.org/][3]]; LTS should just work.
2. Install TypeScript compiler: `npm install -g typescript`

[3]: https://nodejs.org/

There is additional information at
[https://www.npmjs.com/package/typescript][4].

[4]: https://www.npmjs.com/package/typescript



# A TypeScript `Hello, World!` Example

We will begin with a [C# `Hello, World!` example (`hello-world.cs`)][5],
which mainly demonstrates two concepts:

1. The `Main()` entry method of the program.
2. Writing a string to stdout.

[5]: hello-world.cs

It can be re-written as a
[TypeScript `Hello, World!` example (`hello-world.ts`)][6], and this is
how to compile TypeScript (`hello-world.ts`) to JavsScript
(`hello-world.js`) and execute it:

1. `tsc hello-world.ts`
2. `node hello-world.js`

[6]: hello-world.ts

In TypeScript, the entry point of a program is not defined by a `Main()`
method.  Instead, the whole program is executed from top to bottom.  In
other words, the entry point of a program is the beginning of it.

In addition, TypeScript itself does not dictate how to write data.
Instead, it depends on the environment where the compiled JavaScript is
executed.  With Node.js, `console.log()` writes to stdout; if we were to
execute the `hello-world.js` in a web browser, `console.log()` will
write to the web browser's console.

Therefore, technically, we could craft a
[minimum TypeScript `Hello, World!` example (`hello-world-minimum.ts`)][7].

[7]: hello-world-minimum.ts
