# Show HN: Telescope web-based log viewer update

**Posted by r0b3r4 on 2025-06-26**

Hey HN,

A while back, I shared Telescope — a lightweight web UI for exploring logs stored in ClickHouse using a custom query language called FlyQL. Since then, it has come a long way.

Recent releases (including the latest v0.0.19) added several new features:

- **Docker sources:** Browse logs from your running containers directly from the Docker API.
- **Saved views:** Preserve filters, layout, and other UI settings across sessions.
- **Raw SQL mode:** Write plain `WHERE` clauses directly (access to raw mode is permission-controlled).
- **ClickHouse JSON support:** Includes quoted paths and nested field access.
- **Improved FlyQL:** Now easier to read and write, supporting spaces and quoted JSON paths.
- **Miscellaneous improvements and bug fixes:** Smaller tweaks to enhance stability and usability.

Telescope is self-hosted and open-source (MIT license). I’m always happy to receive feedback, feature requests, or GitHub stars!

- **GitHub:** [https://github.com/iamtelescope/telescope](https://github.com/iamtelescope/telescope)
- **Documentation:** [https://docs.iamtelescope.net](https://docs.iamtelescope.net)
- **Demo:** [https://demo.iamtelescope.net](https://demo.iamtelescope.net)
- **Previous post:** [https://news.ycombinator.com/item?id=43181862](https://news.ycombinator.com/item?id=43181862)