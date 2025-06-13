# Show HN: Tattoy – a text-based terminal compositor

**Posted by tombh on 2025-06-13**

---

Tattoy is primarily a terminal eye-candy project designed to impress with its aesthetics, but it also tackles some serious issues.

One of its key features is improving text contrast. For example, when you list a broken symlink with `ls` and see a red background that clashes with your theme's foreground color, Tattoy addresses this by applying the web's WCAG 2.1 contrast algorithm to ensure accessible, high-contrast text.

Another explicit goal of Tattoy is to act as a polyfill for new terminal protocols—effectively becoming the "xwayland" of the TTY. This means you can experiment with deprecating traditional ANSI codes. Applications using new protocols can run within Tattoy, which itself operates in any standard ANSI terminal emulator. More about this concept can be read here: [https://tattoy.sh/news/an-end-to-terminal-ansi-codes/](https://tattoy.sh/news/an-end-to-terminal-ansi-codes/).

Ultimately, Tattoy has been more like an art project—crafted for the sheer pleasure of visual and aesthetic exploration.