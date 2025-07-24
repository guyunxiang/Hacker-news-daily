# Show HN: DrinkMe – A Minimalist Video Compressor

**Posted by wasivis on 2025-07-23**

I recently built my first Electron.js app, a minimalist video compressor called DrinkMe. It uses a two-pass FFmpeg encoding process and estimates the final size based on the video's original duration, resolution, quality, and size.

The idea behind it is to offer an alternative for non-power users who find CLI-based tools like FFmpeg or even GUI programs like HandBrake overwhelming due to their myriad settings and options.

The target compression rate is typically around 80–85% of the original size for high-resolution files, but it adjusts dynamically if the video is already compressed.

All feedback is welcome!