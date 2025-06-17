# Show HN: Chawan TUI web browser

**Posted by shiomiru on 2025-06-16**

A terminal-based web browser written in Nim. It offers acceptable (YMMV) CSS rendering, some JavaScript support, and inline images via sixel/kitty protocols. Additionally, it supports various protocols beyond HTTP(S), such as FTP, Gopher, Gemini, and more.

Chawan originally started as a clone of w3m, and its user interface still resembles it. However, the architecture differs significantly: pages are loaded in separate processes, and protocol/file type handling is delegated to external binaries. This design allows for features like registering decoders for custom inline image formats, though practical use cases remain limited.

You can view a gallery showcasing some websites rendered with Chawan here:  
[https://chawan.net/gallery/index.html](https://chawan.net/gallery/index.html)

[1]: https://nim-lang.org