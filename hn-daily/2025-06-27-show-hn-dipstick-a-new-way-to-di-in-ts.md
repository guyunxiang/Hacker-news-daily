# Show HN: Dipstick – A new way to DI in TS

**Posted by xxiem on 2025-06-27**

For whatever reason, every attempt at Dependency Injection (DI) in TypeScript that I’ve encountered over the last few years is essentially a port of existing DI frameworks from languages like C# or Java/Kotlin. These approaches leave a lot to be desired. Since JavaScript doesn’t have TypeScript types available at runtime, these frameworks tend to hack around that limitation by muddying up the source code with decorators or by creating unique tokens to represent types. I find these hacks pretty ugly.

What’s worse, they violate the principle of least surprise—especially for developers who aren’t familiar with DI—and often produce code that isn’t fully type-safe.

---

**Dipstick** takes a completely different approach by leveraging the TypeScript type system and code generation.

### Key Features

- **Simple**: There are only two concepts to learn—Modules and Bindings.
- **Obvious**: Want to see where a class is instantiated? Use your IDE’s tools. No tricky reflection or magic—just readable, generated code.
- **Modular**: Define multiple modules and compose them together to keep your code organized.

---

The framework is still in early stages and currently supports only classes (which is a limitation). However, if it gains traction, I plan to add support for injecting functions or other literal values.

I’d really appreciate your feedback to help improve Dipstick!