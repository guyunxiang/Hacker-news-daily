# Show HN: CareerCupid now (OkCupid for Jobs) now supports job listings

**Posted by rglullis on 2025-07-01**

I've mentioned CareerCupid [0], a website where people can discover potential co-workers and companies that share their values. It can serve as a kind of screening system without requiring applicants to apply for specific positions.

To address the chicken-and-egg problem, the platform integrates with ActivityPub. You can follow @thecupid@cupid.careers (not a Mastodon bot but a full application built on my Django ActivityPub Toolkit [1]). I demonstrated this integration at the last FediForum, showcasing how we can leverage the existing social graph for building applications, rather than trying to grow the Fediverse by recreating traditional social networks.

Initially, I offered a discount for the first companies to join, but it didn't gain much visibility. Now, as we start a new month and "Who is hiring?" threads are trending, I want to share that company pages and job listings are also integrated with ActivityPub. To celebrate, I’ll be offering the first 100 signups three months free using code **HN2025**.

If you're interested, create an account and set up a "company page" here: [https://cupid.careers/company/new](https://cupid.careers/company/new). After creating the page, you'll see an option to complete the subscription and apply the discount code.

---

CareerCupid functions similarly to how OkCupid used to: users answer questions, indicating (a) how they want others to respond and (b) how important each answer is to them. Comparing answers across users generates a "compatibility score," which could help assess how well you'd get along with potential co-workers.

I'm also developing a "Skill Tree" feature. Its goal is to clarify which parts of a tech stack are critical versus those that can be learned on the job or adapted from related skills. For example, the expectations around "experienced with Python and PostgreSQL" differ greatly between a data analyst, a web backend developer, or a DBA. The Skill Tree would categorize skills into broad categories (e.g., Software Development, Management, UI/UX, System Administration) and branch into more specific skills (e.g., Software Development → JavaScript → React → React Native). This approach allows for flexible, broad, or highly specific skill requirements.

Additionally, I’m considering ideas like creating a database of issues in open-source projects to aid skill assessment, and a more robust "vouching" system where professionals can refer candidates even if they're not currently working at the company. But first, I want to grow the user base and gather feedback.

---

[0]: https://cupid.careers  
[1]: https://activitypub.mushroomlabs.com  
[2]: https://spectra.video/w/nibHzQxR26zQX1eYkFgygL?start=2m44s