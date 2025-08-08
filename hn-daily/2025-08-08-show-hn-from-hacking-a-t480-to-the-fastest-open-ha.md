# Show HN: From Hacking a T480 to the Fastest Open-Hardware 75 Hz E-Ink Display

**Posted by alex-a-soto on 2025-08-08**

Three years ago, I shared my project of hacking together a fast e-ink laptop based on a ThinkPad T480 because I was tired of spending all day on LCD screens. I loved e-ink’s readability and comfort, but its slow refresh rate made it impractical for everyday use.

That initial post attracted a community of enthusiasts who experimented to make e-ink more usable for daily computing. Over time, this effort grew into a company and a multi-year project focused on making e-ink faster and open.

We built our own FPGA-based controller, called Caster, and went through multiple iterations to push beyond e-ink’s typical limitations—such as slow refresh times, ghosting, and reliance on proprietary controllers.

Now, after three years, we’re excited to announce the release of the Modos Paper Developer Kit and Monitor: the fastest open-hardware e-ink display, featuring a 75 Hz refresh rate and sub-100 ms latency.

This hardware supports 6" to 13.3" monochrome or color panels via HDMI or USB-C, offers multiple grayscale modes, and includes a C API for low-level control.

The hardware, firmware, and schematics are available on our [GitHub repository](https://github.com/Modos-Labs/Glider).

Our mission is to make e-ink fast and open enough that anyone can build on it—whether for hacking, research, or daily use.

Thanks, Hacker News, for being part of this journey!