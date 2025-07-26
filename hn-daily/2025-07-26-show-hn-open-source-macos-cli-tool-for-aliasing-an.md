# Show HN: Open-source macOS CLI tool for aliasing and timing command line runs

**Posted by frankbyte on 2025-07-26**

I’m a developer working across multiple tech stacks. At some point, I got tired of typing and remembering lengthy commands for building, testing, and other tasks. To simplify my workflow, I created a small command-line tool that lets me use simple aliases like `ez build` or `ez test`, regardless of the tech stack my repo is based on. (This isn’t magic—it stores the commands once, so I only need to remember the aliases.)

A handy feature I added is that `ez` outputs the time it took to run the subprocess. This is great for monitoring build times and test durations without extra effort. The tool also supports running commands in parallel as separate subprocesses.