# Show HN: I Made a "Block Blast" Solver

**Posted by xFixItNow on 2025-08-09**

I’ve been hooked on the mobile game *Block Blast*! It’s similar to Tetris, but with a twist: you place pieces anywhere on the board. The game ends when you can no longer fit any of your three available pieces.

After a couple of weeks of playing, I built a browser-based solver in HTML/JavaScript that finds the optimal placements for the current pieces. It simulates every possible sequence and selects the one with the smallest perimeter of empty space. In case of ties, it prioritizes layouts with the fewest isolated gaps.

Using this solver, I managed to increase my high score from 36,000 to over 80,000 — and I believe I could have gone even further.

You can try it here: [https://www.adriclumma.com/projects/blockBlastSolver/](https://www.adriclumma.com/projects/blockBlastSolver/)

I'd love to hear what you think — and if it works as well for you as it did for me.