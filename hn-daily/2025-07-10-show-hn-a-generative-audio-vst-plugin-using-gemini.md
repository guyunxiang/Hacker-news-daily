# Show HN: A generative audio VST plugin using Gemini API, JUCE, and React

**Posted by DesaiAshu on 2025-07-10**

Hey folks!

I've spent the last 8 months building a VST plugin called *The Infinite Crate* on top of Magenta's Lyria RealTime music model via the Gemini API. Doug Eck's research group has been developing MusicLM and its variants since 2017. [Watch their related work here](https://www.youtube.com/watch?v=yz-fHidp1M8).

I bridged a JUCE/C++ audio processing foundation with a React/TypeScript UI, using Zustand to sync state. The plugin streams generated audio from the Lyria RealTime model in real-time via WebSockets.

You can try it as a VST3 on Mac/Windows or as an AU/Standalone app on Mac. It works in DAWs like Ableton and Logic, and possibly in other software such as DaVinci Resolve.

The plugin allows you to:
- Enter text prompts
- Adjust generation parameters like top-k, temperature, BPM, key
- Apply various mutes

Please give it a try and share your feedback! 😊

More info: [https://magenta.withgoogle.com/infinite-crate](https://magenta.withgoogle.com/infinite-crate)