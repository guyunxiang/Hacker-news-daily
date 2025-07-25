# Show HN: Building "Love at First Mic" – Tech Clone of TV Show "Love Is Blind"

**Posted by fcpguru on 2025-07-24**

If you're familiar with the show *Love is Blind*, this concept is similar but entirely internet-based. Using vdo.ninja, OBS (Open Broadcasting Software), and some JavaScript, I believe I have all the components to make this work.

You can try it out here: [https://andrewarrow.dev/love-at-first-mic/](https://andrewarrow.dev/love-at-first-mic/)

### How it works:
- At the bottom of the page, enter the invite code **"88c5_48c4_8cf6"**. This will generate two iframes on the page.
- Accept the request for microphone and camera access (if you dare!).
- Another person can enter the same invite code, select "Person B," and they'll see their own camera in one iframe (left side) and a blank black box on the other side. Despite the black box, audio from the other person streams through.
- Meanwhile, the producer (me) opens OBS on a desktop and uses the same invite code to add each person's full video and audio sources via the "Browser" source option in OBS. This allows cropping, scaling, and positioning the videos side by side, then saving everything as a recording.

### The best part:
- No backend server required—completely free!
- I've tried to prevent users from turning off the other's camera by disabling JavaScript and right-clicking, but a determined user could still find ways to cheat.

### What do you think, hackers?
- Has something like this been done before?
- Anyone interested in being the first participant for a "Love at First Mic" season?

Let me know!