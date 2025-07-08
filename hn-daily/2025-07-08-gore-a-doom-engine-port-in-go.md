# Gore – A Doom Engine Port in Go

**Posted by EstIgnavus on 2025-07-08**

Hi HN,

I've been working on Gore — a port of the classic Doom engine written entirely in Go. It's based on a ccgo C-to-Go translation of Doom Generic. Gore loads original WAD files and uses a software renderer, with no dependencies outside the Go standard library — no SDL, CGO, or external libraries. 

There's still some unsafe code that I’m trying to eliminate, along with some other caveats.

In the examples, there's a terminal-based renderer. It’s quite entertaining, even though terminal-style input and output make gameplay challenging.

The goal is to create a clean, cross-platform, Go-native version of the Doom engine that’s fun to hack on, easy to read, and portable.

Code and instructions are available at [https://github.com/AndreRenaud/Gore](https://github.com/AndreRenaud/Gore).

I’d love to hear your feedback or thoughts.