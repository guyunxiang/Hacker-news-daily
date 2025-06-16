# Show HN: Zeekstd – Rust Implementation of the ZSTD Seekable Format

**Posted by rorosen on 2025-06-15**

Hello,

I’d like to share a Rust implementation of the Zstandard seekable format I’ve been working on.

Regular Zstd compressed files consist of a single frame, meaning you have to start decompression from the beginning. The seekable format breaks compressed data into a series of independent frames, each compressed separately. This allows for seeking within a compressed archive: decompressing a section in the middle only requires decompressing at most one frame's worth of data, rather than the entire archive.

I started working with the seekable format because I wanted to resume downloads of large Zstd compressed files that are decompressed and written to disk on the fly. Initially, I created bindings to the upstream C functions available [here](https://github.com/facebook/zstd/tree/dev/contrib/seekable_format). However, I quickly ran into a segmentation fault (now fixed), and I found that these functions only support basic operations. 

Looking closer, I noticed the upstream implementation relies on deprecated core API functions and doesn’t provide access to low-level (de)compression contexts. It appears to be more of a proof-of-concept or demo rather than a maintained production API, which likely explains its placement in the contrib directory.

My use case required a complete rewrite of the seekable format. So, I decided to implement it from scratch in Rust, using bindings to the advanced Zstd compression API available from version 1.4.0.

The result is a simple library crate with a single dependency ([zeekstd](https://crates.io/crates/zeekstd)) and a CLI tool ([see here](https://github.com/rorosen/zeekstd/tree/main/cli)) that functions similarly to the regular Zstd command-line tool.

Feedback is highly appreciated!