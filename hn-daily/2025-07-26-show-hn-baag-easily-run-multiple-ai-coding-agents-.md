# Show HN: Baag – Easily run multiple AI coding agents on the same project

**Posted by pranav7 on 2025-07-26**

I realized I was working on multiple parallel tasks with coding agents, but managing branches in git became a significant bottleneck. I tried Git Butler, but it only complicated things further. Then I discovered git worktrees as a solution, but the git API was a bit too complex for daily use.

So, I decided to build a simple CLI utility to manage the process. It’s designed to work with any setup—whether you're using Claude, Codex, Gemini, Cursor, Vim, or any other tool. The utility mainly manages git worktrees inside your repo and helps set up your development environment the way you like it.

It’s nothing fancy—just a tool I built to scratch my own itch. I figured others might face similar workflow friction, so I wanted to share it here.