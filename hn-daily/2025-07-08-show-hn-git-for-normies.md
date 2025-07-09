# Show HN: Git for Normies

**Posted by sirbread on 2025-07-08**

---

When I was younger, around 10 years old, I remember repeatedly going into the `%AppData%` folder in Windows to take "snapshots" of my Minecraft worlds. I’d copy the world files into a folder and add a timestamp to keep track of versions. Honestly, it got pretty tedious.

A few days ago, I saw my brother doing something similar. Instead of Minecraft worlds, he was backing up image files by making copies and storing them in a folder. He's a digital artist, and when I asked him if he had heard of Git, he responded with, "What in the hacker crap is this?!"

That got me thinking—if Git exists but isn’t very user-friendly for non-power users, what if I created a GUI-based version manager? I’ve seen classmates in high school mess around with Google Docs’ version history; maybe something like that could be useful for local files.

Over the past few days, I built a simple tool I call **"be kind, please rewind."** Remember those stickers from Blockbuster cassettes?

## What is it?

It's a lightweight, local-only versioning tool that runs in the system tray. You point it at a file or folder, and it automatically saves snapshots whenever a file changes—or on a timer if you prefer. There’s no command line, no staging, no commits, no pushes. Just a straightforward safety net you set up once and forget.

## Features

- **Automatic Snapshots:** Detects file changes and snapshots them automatically.
- **Preview Pane:** For images, it shows previews; for text files, a side-by-side diff viewer.
- **Notes & Custom Names:** You can add notes to each snapshot and label them with custom names like "first draft" or "before trying the new thing."
- **Simple Interface:** No complex VCS commands—designed for ease of use by designers, writers, students, and beginner developers working on single files.

## Technical Details

- Built with Python and PyQt5.

I’d appreciate it if you’d take a look!

## Links

- Source code: [GitHub](https://github.com/sirbread/be-kind-please-rewind)
- Binary release: [Releases](https://github.com/sirbread/be-kind-please-rewind/releases/tag/bkpr-v1.0)