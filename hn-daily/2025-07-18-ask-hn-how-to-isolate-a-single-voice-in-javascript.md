# Ask HN: How to isolate a single voice in JavaScript?

**Posted by pas256 on 2025-07-18**

I'm developing a two-player game where each player uses their phone as a microphone. The setup works well when players are not talking at the same time, but a big issue arises when they speak simultaneously. It turns out that the iPhone microphone is highly effective at picking up all voices in the same room.

I've set `echoCancellation: true` and `noiseSuppression: true` in my `AudioConstraints`, but I believe those settings are intended for different purposes.

Does anyone have ideas on how to solve this?