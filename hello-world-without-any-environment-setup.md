# `Hello, World!` without Any Environment Setup

Let's go thru a `Hello, World!` example without any environment setup.



# TypeScript Playground

1. Go to [https://www.typescriptlang.org/play/][1]
2. In the text area on the left, copy and paste the `Hello, World!`
   example below.
3. Click the `Run` button above the text area on the right.  The
   `Hello, World!` example will be executed, and its output should
   appear in a new web browser window.

[1]: https://www.typescriptlang.org/play/



# A TypeScript `Hello, World!` Example

This is what a C# `Hello, World!` example may look like.

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

The C# `Hello, World!` example above can be re-written in TypeScript
like this:

```
// A TypeScript `Hello, World` example.
class C {
    static aStaticMethod(): string {
        return "Hello, World!";
    }
}

document.body.textContent = C.aStaticMethod();
```

Notice that TypeScript does not have a `Main` entry method.  Instead,
TypeScript code is executed from top to bottom.  Therefore, a minimum
TypeScript `Hello, World!` example may look like this:

```
document.body.textContent = "Hello, world!";
```
