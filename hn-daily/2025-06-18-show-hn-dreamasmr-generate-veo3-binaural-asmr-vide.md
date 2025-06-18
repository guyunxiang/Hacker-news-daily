# Show HN: DreamASMR – Generate Veo3 Binaural ASMR Videos from One Prompt

**Posted by howardV on 2025-06-18**

Hi HN,

I recently pivoted a generic video-generation side project into *DreamASMR* — a web app that transforms a text prompt into a fully download-able, 16:9 ASMR video with true binaural audio in about 30 seconds.

## Why niche down to ASMR?

- Slicing, pouring, tapping videos dominate the “oddly satisfying” niche; high-quality audio is crucial but underserved.
- Veo3’s macro rendering and high FPS outperform SD/Sora for tiny textures like glass, sand, or honey.
- Most existing tools lack a licensing pathway for commercial ASMR creators.

## Key features

- **Prompt enhancer:** Automatically adds acoustic and visual context to help beginners achieve good results.
- **Binaural pipeline:** Converts mono output from Kie.ai into stereo left-right sound, optimized for headphone experience.
- **One-click download:** Videos are stored on Cloudflare R2 with a server proxy to bypass CORS issues.
- **Credit billing:** Charges only 1 credit upon successful video generation; zero credits if it fails.

## Tech stack

- Next.js (App Router, mainly server components) + Tailwind + Shadcn
- Veo3 API via Kie.ai proxy
- PostgreSQL + drizzle-orm
- Cloudflare R2 for storage
- Next-Auth (Google/Email)
- Cloudflare Turnstile to block bots
- 100% TypeScript with minimal client-side JavaScript

## Demo

[https://dreamasmr.com](https://dreamasmr.com)

## Looking for feedback on

1. **Generation quality:** Which objects or sounds still feel off?
2. **Prompt UX:** Do you prefer a simple text box or template presets?
3. **Pricing:** Would you pay for professionally licensed ASMR loops?
4. **Performance & architecture:** Any bottlenecks in large file downloads or handling high concurrency?

## Roadmap

- Perfect-loop mode
- Pure audio ASMR generator
- WebM with alpha channel for compositing
- Public API/SDK

Thanks for reading! Looking forward to your thoughts and feedback!