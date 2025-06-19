# Show HN: universal application where LLM does all computation directly

**Posted by snickell on 2025-06-18**

Universal is a demonstration of a *universal application* ("OS") where all computation is performed directly by the LLM. This concept is similar to the ideas recently discussed by Karpathy in his YC AI SUS talk.

The system operates on a loop where user commands or mouse clicks are fed into the LLM. The LLM is instructed to render the next frame, treating it as if it were rendering a frame of a video. In this implementation, static HTML and CSS are used to represent the "image," since current LLMs do not produce high-quality text fidelity in image outputs.

In essence, computation is handled entirely by the LLM itself — it is not just writing code but *is* the code.