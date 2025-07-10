# Show HN: I added A/B testing to my cold email generator – does this add value?

**Posted by ZeeeTH on 2025-07-09**

I built ColdCopy (coldcopy.xyz) a few days ago to solve my own cold email writing struggles. Initially, it generated a single personalized email, but I kept wondering, "Should this be more direct or more friendly?"

So, I added A/B testing. Now, it generates three versions—Professional, Friendly, and Direct—side-by-side so you can compare and choose the best approach.

Early users seem to like having options, but I’m curious if this feature is genuinely useful or just extra bloat. Does having multiple versions actually improve cold outreach, or does it lead to decision paralysis?

The technical implementation was straightforward: same form data, three API calls with different prompt variations, and a responsive grid to display the results. But I’m more interested in whether this solves a real problem.

ColdCopy is built with Next.js 14 and the OpenAI API. It’s currently free with daily limits.

What do you think—is A/B testing for cold emails useful, or am I overthinking this?