# Show HN: Web page animation library for all frameworks

**Posted by rhdclrl on 2025-07-25**

---

Ever notice how native mobile apps have those buttery smooth transitions when navigating between screens? Instagram stories, WhatsApp chats, any modern mobile app really. Meanwhile, web pages still feel clunky with their instant page loads.

I built *SSGOI* to bridge that gap — a library that brings native-like screen transitions to web applications.

## Technical Challenges Solved

- **Universal browser support**  
  No reliance on cutting-edge APIs like Chrome's View Transition API. Everything was built from scratch to ensure compatibility across all browsers.

- **SSR compatibility**  
  Seamlessly integrates with frameworks like Next.js, Nuxt, and others without breaking hydration or causing layout shifts.

- **Drop-in integration**  
  Zero refactoring needed. Just add the library to existing projects without touching your routing logic or application structure.

## Framework-Agnostic Approach

Built to work with React, Vue, Svelte, Angular, or vanilla JavaScript. The core engine handles the heavy lifting, while framework-specific adapters provide the necessary integration layer.

## Performance Considerations

- Hardware-accelerated CSS transforms  
- Efficient memory management during transitions  
- Minimal bundle size impact  
- Configurable transition duration and easing

The goal was simple: make web navigation feel as polished as native apps without sacrificing performance or developer experience.

## Find out more

[https://github.com/meursyphus/ssgoi](https://github.com/meursyphus/ssgoi)

Open to feedback and contributions. If you find this useful for your projects, I’d appreciate any stars.