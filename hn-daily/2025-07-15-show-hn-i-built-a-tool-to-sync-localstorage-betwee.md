# Show HN: I built a tool to sync localStorage between devices

**Posted by meistertigran on 2025-07-15**

At my day job, we have a daily async stand-up. We need to message a Slack bot with how many hours we've worked on each task that day and in total.

The format is:
> Task: "Task Name" | Worked: 5h | Total: 16h  
> Description: Finished implementation of feature.

I don't complain—most fully remote jobs have some version of this process, but doing it manually got tedious. I wanted a simple app to track this data effortlessly.

I'm not usually a fan of “vibe-coded” apps, but this was an ideal candidate since it’s not meant for production. Most large language models (LLMs) approach this by creating a single HTML file with forms that save data to localStorage. That worked perfectly for me—no hosting, no database, no backend needed. Just 15 minutes of prompting.

One day, while outside with only my phone, I realized I couldn’t use the app. I thought, “How hard can it be to synchronize localStorage data across devices?” Turns out, it’s not that hard if you're willing to build a platform around it.

I built [htmlsync.io](https://htmlsync.io), which does just that. You upload your HTML app that uses localStorage and get a custom subdomain. The platform automatically synchronizes your changes across devices. You can create private or public apps, choose which keys to sync using the `no_sync_` prefix, and hide UI elements in public views with the `public-hidden` CSS class. It also provides a subdomain profile page listing all your apps for easy access.

I hope you find this as useful as I did.  
I’d love to hear your feedback if you decide to try it out.