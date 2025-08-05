# Show HN: I built the fastest VIN decoder

**Posted by samsullivan on 2025-08-04**

I’ve developed a VIN decoder that processes any VIN in approximately 20 milliseconds, with no need for network calls. I achieved this by compressing the entire NHTSA vehicle database into a 21MB SQLite file that runs entirely offline.

There are no API keys, rate limits, or servers involved. You just download it once, and you can decode VINs indefinitely. It works in browsers, Node.js, Cloudflare Workers—anywhere SQLite is supported.

I’d love to get any feedback and answer questions about the implementation.