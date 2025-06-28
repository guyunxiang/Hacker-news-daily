# Show HN: USB Connection Info – Mac Menu Bar App to Avoid Cable Confusion

**Posted by tTarnMhrkm on 2025-06-27**

Like many of you, I’ve collected a drawer full of USB-C cables over the years. I’ve also experienced the frustration of plugging in a "fast" external SSD only to see abysmally slow transfer speeds.

Recently, I got a new SSD, eager to perform quick backups. I plugged it in, started copying, and watched the transfer progress crawl for hours on just a few gigabytes. My immediate thought: the drive is DOA, or worse, I was scammed.

After some head-scratching and cable swapping, I discovered the culprit: a USB-C cable that negotiated only USB 2.0 speeds. It looked identical to my other cables, but its internal wiring limited the transfer rates. This is a common problem, made worse by the visual similarity of USB-C cables despite their vastly different capabilities.

I knew macOS’s System Information panel could show the current USB connection speed, but checking that every time I connected a device or swapped cables was too cumbersome for my workflow. I wanted a better solution.

**So, I built one.** 

Having developed several Mac apps in Swift before, I took on the challenge of creating a lightweight, background menu bar application. The goal was to provide quick, at-a-glance USB connection info without digging through system panels.

The result is **USB Connection Information**, a small menu bar app that displays the active USB connection speed, USB version, wattage, device manufacturer, and more. No more guessing or deep system dives—just immediate insight.

It’s now available on the Mac App Store, supporting macOS 13.0 and later.

You can find it here: [https://apps.apple.com/app/id6747853674](https://apps.apple.com/app/id6747853674)

I’d love to hear your thoughts and feedback. Has this been a problem for you too?