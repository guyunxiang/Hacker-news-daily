# Show HN: Yet Another Kanban – FOSS, local, private project management

**Posted by mackenziebowes on 2025-07-28**

I created a free, local, private Kanban tool and published the source code. To provide more details on how it works, my inspiration, and potential use cases, I also made a video:

[Watch the video](https://www.youtube.com/watch?v=6qJYg3OuOx4)

I built this to support my work on another project. I had that classic moment of frustration over paying $20 a month for a SaaS Kanban, but I managed to develop my own solution in just two days—thanks to a sick component library.

### What makes this Kanban different?

- **Progressive enhancement pattern**: Uses a popular Japanese mobile-to-desktop approach often seen outside America.
- **Markdown support with gfm-md**: Enables easy dumping of tickets from ChatGPT, Claude, Gemini, etc.
- **Local storage with SQLite**: Everything runs locally for privacy and control.
- **Flexible development**: You can run `bun dev --host` to develop on your phone while working around your office.
- **Ready-to-use hooks**: Includes database schemas and routes for adding authentication, making deployment straightforward. You can host it on a $12 Akamai box or a cheaper alternative—subscribing to SaaS costs can be avoided.

Use **bun** as the runtime for this project.

Enjoy saving between $96 and $240 annually! :3