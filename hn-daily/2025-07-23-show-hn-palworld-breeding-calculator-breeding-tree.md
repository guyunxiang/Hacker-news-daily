# Show HN: Palworld Breeding Calculator – Breeding Tree and Combination Visualizer

**Posted by droidHZ on 2025-07-23**

Hi HN! I’m an indie developer who got hooked on Palworld’s breeding system and built a tool to make planning less painful:

## What it does

- **Forward calculation:** Pick two parents to instantly see the resulting child.
- **Reverse lookup:** Enter a target Pal to get a list of all valid parent pairs.
- **Shortest-step planner:** Models breeding as a graph and uses a shortest-path algorithm (Dijkstra/BFS variant) to find the minimal number of steps from what you already own to your target.
- **Breeding tree visualizer:** Expand and collapse an interactive tree of possible combinations to understand the breeding route at a glance.
- **Combination browser:** Search and filter all possible parent-child sets.

## Tech bits

- Built with Next.js, using static JSON data scraped and cleaned from public sources.
- Deployed on Vercel and Cloudflare.
- Uses precomputed indices for fast reverse lookups, along with client-side memoization and caching.
- The graph layer treats each Pal as a node; edges represent “(A,B) → C” relationships. Since these are hyperedges, I flatten them into a weighted graph so a shortest-path algorithm can run efficiently.
- No trackers or popups; just a single AdSense slot (feedback welcome on this).

## What I’d love feedback on

- **UX:** Is the flow from “I have X and want Y” smooth enough?
- **Performance/Mobile:** Are there obvious bottlenecks?
- **Data correctness:** Are there inaccuracies or missing combos?

## Link

[https://www.palworldbreedingcalculator.org/](https://www.palworldbreedingcalculator.org/)

Thanks for reading! I’ll be around to answer questions and ship fixes quickly.