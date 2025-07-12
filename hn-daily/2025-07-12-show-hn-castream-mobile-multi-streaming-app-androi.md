# Show HN: Castream – Mobile Multi-Streaming App (Android Live, iOS in Beta)

**Posted by acabralto on 2025-07-12**

Hi HN — I built [Castream](https://castream.io), a native mobile app for multi-streaming live video to platforms like YouTube, Facebook, Twitch, and more — directly from your phone.

Android is available now on the Play Store, and iOS is currently in beta.

I created this because I was frustrated with relying on OBS setups and clunky desktop workflows just to stream to multiple destinations. Castream allows you to go live in seconds, with native camera and mic capture, high-quality video, and automatic restreaming handled server-side.

## Tech Stack
- React Native app with native video and audio modules
- Hardware-accelerated encoding using MediaCodec and FFmpegKit
- FastAPI backend with Redis and MySQL
- Kubernetes-powered video processing for ingest, transcoding, and fan-out

I’d love feedback from anyone who has streamed before or is into media infrastructure. To encourage early adoption, I’m offering a free month of the Pro tier — no paywalls or hidden catches. Just trying to make mobile streaming genuinely usable.