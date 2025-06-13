# Show HN: Tool-Assisted Speedrunning the Boring Parts of Animal Crossing (GCN)

**Posted by hunterirving on 2025-06-12**

I recently dug my Nintendo GameCube out of storage to revisit the first Animal Crossing game. Things were mostly as I remembered, but the game's heavy reliance on a clunky on-screen keyboard quickly tested my patience.

Unwilling to accept this subpar experience, I ordered a rare, Japan-exclusive keyboard/controller hybrid on eBay. Using a Raspberry Pi Pico, I:

- Listened for keypresses
- Sent simulated controller events to the GameCube

This setup allowed me to automate typing in Animal Crossing at a Tool-Assisted Speedrun (TAS) level.

Since the oddball controller’s keycaps didn't match Animal Crossing's in-game character set perfectly, I watched a 10-hour FreeCAD tutorial at 2x speed. I modeled 7 keycap profiles to create 81 custom, 3D-printed keycaps, including esoteric Greek and Old English characters Nintendo had included.

Having solved my initial problem, I looked for new challenges. I used my TAS device to automate entering customizable "Town Tune" melodies, exploited a cracked encryption algorithm to access nearly every in-game item, and whipped up a Python script to convert arbitrary images into the game’s 32x32 pixel custom design format.

Inputting 1024 pixels even at superhuman speed took about 3 minutes, but I extended the concept to video. I playback Rick Astley's "Never Gonna Give You Up," Bad Apple!, Shrek, and even a short DOOM clip—though rendering 30 seconds of footage at 5 fps took around 7.5 hours.

Realizing that running DOOM at approximately 0.0056 fps isn’t exactly playable, I decided to get a simple game running within Animal Crossing—to my surprise, it was Snake.

Since Snake only needs to update one pixel per frame, I managed to run it at around 1 fps (variable due to technical reasons). It’s not the most polished gaming experience, but it’s definitely a game. It even keeps an in-memory high score, and so far, I’m undefeated.

The code and design files are free on GitHub [here](https://github.com/hunterirving/pico-crossing). A build and demonstration video is available on YouTube [here](https://www.youtube.com/watch?v=Yw8Alf_lolA).

What started as a "quick, simple project" quickly ballooned into several more, but I had a blast putting it all together. Thanks for checking it out!