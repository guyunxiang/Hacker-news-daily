# Show HN: Castream – Native iOS/Android IRL Multistreaming App

**Posted by acabralto on 2025-07-18**

Hey HN,

I just launched the iOS version of Castream, a native app that allows you to multistream directly from your phone to platforms like Twitch, YouTube, Facebook, and any custom RTMP endpoint. Android has been live for a while — iOS just went live this week.

This app was built to address common mobile streaming challenges: unreliable apps, lack of multistream support, or the hassle of using a PC. Castream uses native encoding and streams directly from your phone via real RTMP — no browser wrappers or WebRTC hacks involved.

### Key Features:
- Native iOS and Android apps with hardware-accelerated video and audio encoding
- Multistreaming with your own RTMP keys
- Free plan: supports 720p to two destinations, up to 5 minutes per stream
- Paid plans: unlock 1080p, more destinations, unlimited streaming time, and additional features
- Backend built with FastAPI, utilizing FFmpeg on-device for muxing and streaming
- Developed solo — full stack and native mobile (Swift, Java, Kotlin)

We’re currently gaining early sign-ups mostly through organic reach—we haven't run any ads yet. Our focus is on attracting real users and gathering feedback.

### Links:
- [iOS App](https://apps.apple.com/app/castream/id6747093725)
- [Android App](https://play.google.com/store/apps/details?id=io.castream.app)
- [Website](https://www.castream.io)

Would love to hear any feedback, especially from those working in video, streaming infrastructure, or native mobile development.

Thanks!