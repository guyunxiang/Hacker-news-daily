# Show HN: I recreated 90s Mode X demoscene effects in JavaScript and Canvas

**Posted by gneissguise on 2025-06-17**

After 25 years of writing software, I was feeling nostalgic for the kinds of projects that first got me into programming: the old DOS demoscene. I spent a weekend experimenting to see if I could recreate some of that classic INT 13H VGA magic using modern web technologies, but with the constraints of starting from scratch.

The result is a portfolio of ten classic effects all contained within a single HTML file. It’s built entirely with vanilla JavaScript and a `<canvas>` element, with no external libraries. Implementing these effects was a fun challenge and a great way to revisit fundamental techniques. Some highlights include:

- **Color palette cycling and smooth fading**, as seen in the Plasma demo.
- **Buffer-averaging algorithm** for the Fire effect, creating more natural-looking flames.
- **Distance-based texture crossfading** in the Tunnel effect to simulate flying through different sections.
- **2D scalar field for Metaballs**, calculating surface normals for that iconic blended, metallic look (done within the constraints).

This project was a great exercise in getting back to first principles, and it’s a reminder of how much early demo programmers could accomplish with very limited resources. I hope it brings back some good memories for others who grew up with this style.

I’d love to hear about your favorite classic demos or any iconic effects you think would be fun to recreate. Feel free to suggest challenges or ideas!

Cheers!