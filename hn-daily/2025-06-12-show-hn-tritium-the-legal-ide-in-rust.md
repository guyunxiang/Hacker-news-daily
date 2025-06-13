# Show HN: Tritium – The Legal IDE in Rust

**Posted by piker on 2025-06-12**

Hi HN! I’d like to introduce Tritium ([https://tritium.legal](https://tritium.legal)). Tritium aims to bring the power of an integrated development environment (IDE) to corporate lawyers.

My name is Drew Miller, and I’m a lawyer admitted to the New York bar. Over the past 13 years, I’ve been involved in corporate transactional work while building side projects in various languages using vanilla Vim. One day at work, I was asked to develop a legal technology product at my firm. The only available tools for editing and running programs in a locked-down environment were VS Code and extensions like Puppeteer from Microsoft.

I was blown away by features like "go-to definition," syntax highlighting out of the box, and debugger integration. I immediately switched to a full IDE for my side projects. It then struck me: why don’t we have this same kind of tool in the world of corporate law?

Currently, corporate lawyers spend countless hours navigating multiple applications and countless Word and Adobe windows. The existing differencing products are sub-par, making `patch` look innovative, all while charging exorbitant fees.

A few months later, I left my practice to build Tritium. The goal is for Tritium to be the lawyer’s VS Code — an all-in-one drafting cockpit that treats a deal’s entire document suite as a single, searchable, AI-enhanced workspace. It remains fast, local, and secure.

Tritium is implemented entirely in Rust, making it cross-platform. I’m excited about the possibility of lawyers using Linux as their daily driver. The interface leverages a modified version of the ultra-fast egui.rs immediate-mode GUI library. The Windows build includes a Rust COM implementation, which was one of the more technical challenges besides designing the text layout and rendering.

You can download a copy at [https://tritium.legal/download](https://tritium.legal/download) or try out a web-only WASM preview here: [https://tritium.legal/preview](https://tritium.legal/preview).

I’d love to hear your thoughts! Your feedback is incredibly valuable. Thank you for your time.