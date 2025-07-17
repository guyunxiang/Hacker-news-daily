# Show HN: Visualize Wikipedia link graph, opensourced

**Posted by xinbenlv on 2025-07-17**

---

## Overview

WikiLoop Galaxy is an interactive network visualization tool that maps Wikipedia articles and their connections using the Wikipedia API. Built with D3.js, it allows dynamic graph rendering and real-time exploration of Wikipedia's interconnected articles.

## Web App

[https://galaxy.wikiloop.org](https://galaxy.wikiloop.org)

*Note: There appears to be a formatting issue with the link in the original post; verify the URL before use.*

## Source Code

[https://github.com/wikiloop/galaxy](https://github.com/wikiloop/galaxy)

## Wikipedia Page

[[WP:WikiLoop Galaxy]](https://en.wikipedia.org/wiki/WP:WikiLoop_Galaxy) *(link may vary; check the actual Wikipedia page)*

---

## Demo

![WikiLoop Galaxy Demo](File:WikiLoop Galaxy Demo-v0.0.2.gif)

Watch the full demo on Loom:  
[Full WikiLoop Galaxy Demo on Loom](https://www.loom.com/embed/5ccb54c0ce934939aee0458d23fa0cb2?sid=77210291-f6a8-4351-ac9d-a347152a00db)

---

## Release Notes

See [[Wikipedia:WikiLoop_Galaxy/Release/v0.0.2]] for detailed release information.

---

## Features

### Core Functionality

- **Bidirectional Link Traversal**: Explore both outbound links (from articles) and inbound links (to articles).
- **Real-time Graph Building**: Start from a root article and build the network dynamically.
- **Interactive Expansion**: Click any node to expand it with 10 connected articles.
- **Link Validation**: Checks page existence to handle broken Wikipedia links.

### Visual Design

- **Obsidian-style Dark Theme**: A clean, modern interface optimized for graph exploration.
- **Color-coded Nodes**:
  - Green: Root article (starting point)
  - Blue/Teal: Valid Wikipedia articles (first/second degree)
  - Red: Missing or non-existent pages (red links)
  - Yellow Border: Expandable nodes with pulsing animation
- **Force-directed Layout**: Nodes are positioned naturally using physics simulation.
- **Zoom & Pan**: Navigate large graphs easily with mouse controls.

### Interaction

- **Click**: Expand a node to reveal 10 inbound and 10 outbound links.
- **Ctrl/Cmd + Click**: Open the Wikipedia article in a new tab.
- **Drag**: Move nodes around the canvas.
- **Scroll**: Zoom in and out of the graph.

---

Feel free to try out this open-source project to visualize Wikipedia's rich network of articles!