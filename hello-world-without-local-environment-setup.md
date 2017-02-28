# `Hello, World!` without Local Environment Setup

Let's go through a TypeScript `Hello, World!` example without having to
set up a development environment locally.



# TypeScript Playground

We will take advantage of the official TypeScript online playground.  It
should work with all modern web browsers.

1. Go to [https://www.typescriptlang.org/play/][1]
2. In the text area on the left, copy and paste the `Hello, World!`
   example below.
3. Click the `Run` button above the text area on the right.  The
   `Hello, World!` example will be executed, and its output should
   appear in a new web browser window.

[1]: https://www.typescriptlang.org/play/



# A TypeScript `Hello, World!` Example

We will begin with a C# `Hello, World!` example.  This is what it may
look like.

```
// A C# `Hello, World!` example.
class C
{
    static void Main()
    {
        System.Console.WriteLine("Hello World!");
    }
}
```

This is how it can be re-written in TypeScript.

```
// A TypeScript `Hello, World` example.
class C {
    static getHelloWorldString(): string {
        return "Hello, World!";
    }
}

document.body.textContent = C.getHelloWorldString();
```

The C# `Hello, World!` example above mainly demonstrates two concepts,
and we will examine them in the context of TypeSciprt.

1. The `Main()` entry method of the program.
2. Writing a string to stdout.

In TypeScript, the entry point of a program is not defined by a `Main()`
method.  Instead, the whole program is executed from top to bottom.  In
other words, the entry point of a program is the beginning of it.

In the context of this tutorial, because the `Hello, World!` example
will be executed in a web browser, there is no stdout.  Instead, the
TypeScript `Hello, World!` example writes a string by modifying an HTML
document through [DOM][2].

[2]: https://en.wikipedia.org/wiki/Document_Object_Model

Therefore, technically, a minimum TypeScript `Hello, World!` example
may look like this.

```
// A minimum TypeScript `Hello, World` example.
document.body.textContent = "Hello, World!";
```
