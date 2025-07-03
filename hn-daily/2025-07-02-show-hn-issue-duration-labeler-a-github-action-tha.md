# Show HN: Issue Duration Labeler – a GitHub Action that labels issues by age

**Posted by mireklzicar on 2025-07-02**

I’ve built *Issue Duration Labeler*, a GitHub Action that automatically adds *color-coded duration labels* to every issue in a repository:

- **Default label thresholds:**  
  - Green – ≤ 7 days (configurable)  
  - Orange – ≤ 30 days  
  - Red – > 30 days

For open issues, the action calculates the “age” from creation date to now. You can customize the day thresholds and label colors in the workflow file, and choose whether labels update daily or only when issues cross a threshold.

### Why use it?

I often lose track of how long tickets have been open, especially in older projects. A quick glance at the issue list or GitHub project can now reveal at a glance what’s fresh, what’s getting stale, and what’s long overdue. It’s also useful for post-mortems: sorting by red labels highlights issues that took the longest to close.

### Link

[https://github.com/marketplace/actions/issue-duration-labeler](https://github.com/marketplace/actions/issue-duration-labeler)