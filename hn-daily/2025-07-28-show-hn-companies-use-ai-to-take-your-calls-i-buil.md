# Show HN: Companies use AI to take your calls. I built AI to make them for you

**Posted by michaelphi on 2025-07-28**

We're living in this strange asymmetry: companies are adopting AI voice agents to talk to us, but we're still manually dialing their numbers. Big retail, family dentists, local pharmacies—everywhere you're seeing AI voice assistants in action. This year, I've been in a few calls where the AI sounded incredibly natural, which was pretty cool to experience. It made me wonder—why are we, the consumers, still making the calls if companies are already using robots on their end?

So, I built Piper: an AI that makes phone calls for you. You tell it what you need—schedule an appointment, check an order, dispute a charge, whatever—and it handles the entire conversation, freeing you up to do your actual work. Currently, it’s a web app, and a Chrome extension is pending approval. Soon, you’ll be able to click any phone number anywhere and let Piper handle the call.

### Technical Challenges

- **Latency:** Every millisecond matters in a conversation. I optimized around KV cache, reducing latency to about 1000ms to produce the first word over PSTN. It now feels quite natural.
- **Keeping the voice agent on track:** Built custom context engineering logic that continuously updates the agent’s situational awareness, so it knows when it’s been transferred, put on hold, etc.
- **Performance:** So far, we've completed around 50 successful calls with early testers. Failures mainly occur with complex verifications or documents. We also temporarily took down our IVR navigation to fix some edge cases that caused unnecessary transfers.

### The Future of AI in Phone Calls

I really believe we’re heading toward a world where AI talks to AI for most routine interactions. Phone calls could be the first widespread example of this at scale!

You can check out a voice demo on our website: [https://pipervoice.com](https://pipervoice.com)