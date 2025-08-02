# Tell HN: Gemini CLI is buggy; use at your own risk

**Posted by prmph on 2025-08-01**

Gemini CLI has many bugs, and today I encountered a new class of issues.

I installed it on a new machine, logged in, and asked it to work on a file that has the same name as another file on my original machine. Somehow (I don't even understand how this slipped past QA), it was using the content from the first machine instead of actually reading the file on the new machine.

Additionally, it once kept using an old version of a file I had manually updated, despite me requesting it multiple times to re-read the file.

Overall, it feels like it's not ready for serious use.