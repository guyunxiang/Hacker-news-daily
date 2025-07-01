# Show HN: Local LLM Notepad – run a GPT-style model from a USB stick

**Posted by davidye324 on 2025-06-30**

---

## What it is

A single 45 MB Windows executable that embeds llama.cpp along with a minimal Tk UI.  
Copy it, along with any `.gguf` model file, to a USB flash drive.  
Plug into any Windows PC, double-click, and you can chat with an LLM—no admin rights, no cloud connection, no network required.

## Why I built it

Most existing local LLM GUIs assume you can install via pip, pass long command-line flags, or download gigabytes of extra data.  
I wanted something simple enough that my less-technical colleagues could run during a client visit by just plugging in a USB drive.

## How it works

- Packaged using PyInstaller’s one-file build, bundling Python runtime, llama.cpp Python bindings, and the UI into a single `.exe`.  
- On first launch, it memory-maps the `.gguf` model file; subsequent prompts stream at approximately 20 tokens per second on an i7-10750H with a 0.8 GB model (`gemma-3-1b-it-Q4_K_M.gguf`).  
- The tick-driven render loop ensures the UI remains responsive while llama.cpp processes the prompts.  
- The interface highlights (bold, underline) tokens that originated from the prompt.  
- Ctrl+click on a token opens a "source viewer" to trace facts and help identify hallucinations quickly.  

This setup allows easy, offline interaction with a GPT-style model directly from a USB stick, ideal for quick demonstrations or troubleshooting in environments where installing software isn't feasible.