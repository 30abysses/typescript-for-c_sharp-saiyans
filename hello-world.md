# `Hello, World!`

Let's go thru a `Hello, World!` example.



# Get TypeScript Compiler

There are a few options listed on
[https://www.typescriptlang.org/index.html#download-links][1].  The
Node.js option is the simplest for our purpose.

[1]: https://www.typescriptlang.org/index.html#download-links

1. Install Node.js: [https://nodejs.org/][2]; LTS should just work.
2. Update npm: `npm install -g npm`
3. Install TypeScript compiler: `npm install -g typescript`

[2]: https://nodejs.org/



# A TypeScript `Hello, World!` Example

1. Compile [hello-world.ts][3]: `tsc hello-world.ts` to produce
   `hello-world.js`.
2. Execute `hello-world.js`: `node hello-world.js`
3. You should see `Hello, World!` written to `stdout`.

[3]: hello-world.ts



Notice that

* TypeScript's default class member access modifier is `public` while
  C#'s is `private`.
* TypeScript does not have a `Main` entry method; the code is executed
  from top to bottom.
