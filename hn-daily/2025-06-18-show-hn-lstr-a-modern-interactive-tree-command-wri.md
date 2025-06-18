# Show HN: Lstr – A modern, interactive tree command written in Rust

**Posted by w108bmg on 2025-06-18**

Hi HN,

(First time poster!)

I'm the author of `lstr`. I’ve always loved the classic Linux `tree` command for its simplicity, but I often found myself wanting more modern features like interactivity and Git integration. So, I decided to build my own version in Rust with a philosophy of being fast, minimalist, and interactive. It was also an excuse to learn more about Rust!

Here’s a quick look at the interactive mode:

![Lstr Demo GIF](https://raw.githubusercontent.com/bgreenwell/lstr/main/assets/lstr-demo.gif)

I’ve just released v0.2.0 with some features I think this community might find useful:

- **Interactive TUI Mode**: Launch it with `lstr interactive`. It allows for keyboard-driven navigation, expanding/collapsing directories, and opening files in your default editor.

- **Git Status Integration**: Using the `-G` flag, `lstr` shows the Git status of every file and directory directly in the tree output.

- **Shell Integration**: In interactive mode, you can press `Ctrl+s` to quit and have `lstr` print the selected path to stdout. This enables piping the output into other commands or using it as a visual `cd`. For example, add this function to your `.bashrc` or `.zshrc`:

  ```bash
  lcd() {
      local selected_path
      selected_path="$(lstr interactive -gG)"
      if [[ -n "$selected_path" && -d "$selected_path" ]]; then
          cd "$selected_path"
      fi
  }
  ```

  Just run `lcd` to visually pick a directory and jump to it.

Lstr also supports file-type icons (via Nerd Fonts), file sizes, permissions, and respects your `.gitignore`.

The project is open-source and I’d love to get your feedback.

GitHub: [https://github.com/bgreenwell/lstr](https://github.com/bgreenwell/lstr)  
Crates.io: [https://crates.io/crates/lstr](https://crates.io/crates/lstr)

Thanks for checking it out!