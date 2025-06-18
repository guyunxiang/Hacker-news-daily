# Show HN: Utsuru – "Go Live" simultaneously on multiple Discord calls

**Posted by centverdynanta on 2025-06-18**

Hello there HN! I’d like to share a small project I just built and see if there’s any interest.

## What is Utsuru?

Utsuru is a WebRTC utility that allows you to "Go Live" on Discord using OBS, FFmpeg, or any tool supporting WHIP. It also enables broadcasting to multiple Discord calls simultaneously — so you can stream your content to multiple servers at once.

## The Idea Behind Utsuru

The project started as an effort to better understand WebRTC. From my experience, WebRTC is mainly used for web app projects. I initially set it aside, feeling no need for another broadcasting or video conferencing platform.

Later, I grew frustrated with Discord’s limited stream controls. It’s difficult to stream a specific application with system audio or to customize the layout of streams. I wanted a way to use a compositor—enter OBS.

I discovered OBS’s "Windowed Projector" feature, which lets me set Discord to "Go Live" on a specific application window, then stream that to Discord. But I found this solution kludgy and not very refined.

## Inspiration and Discovery

While exploring related projects on GitHub, I came across the [`Discord-video-stream`](https://github.com/Discord-RE/Discord-video-stream) project. It allows streaming local or buffered files to Discord. That line in its README caught my eye:

> For better stability it is recommended to use WebRTC protocol instead since Discord is forced to adhere to spec, which means that the non-signaling portion of the code is guaranteed to work.

This reminded me of WebRTC’s potential and reignited my initial interest.

## Building Utsuru

The original project used Discord's custom UDP protocol, transcoding files with FFmpeg before sending them to Discord. I realized I could learn WebRTC by building a similar tool, but one that:

- Uses the standard WebRTC protocol
- Accepts input directly from OBS
- Sends streams to Discord without transcoding

Next, I checked if OBS supported WebRTC streaming. It does, under the name WHIP. 

To make distribution simple, I wanted to package everything as a single executable. I chose Rust for development because of my familiarity with it as a compiled language.

## Thanks for Checking Out Utsuru!

I’d love to hear your thoughts or feedback. You can find the project on GitHub:

**GitHub:** [https://github.com/VincentVerdynanta/utsuru](https://github.com/VincentVerdynanta/utsuru)

And for reference, here’s the project that inspired it:

**Related project:** [https://github.com/Discord-RE/Discord-video-stream](https://github.com/Discord-RE/Discord-video-stream)

---

Feel free to explore and give feedback!