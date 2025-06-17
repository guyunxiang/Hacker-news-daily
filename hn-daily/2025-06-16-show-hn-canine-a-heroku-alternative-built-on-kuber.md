# Show HN: Canine – A Heroku Alternative Built on Kubernetes

**Posted by czhu12 on 2025-06-16**

Hello HN!  

I've been working on Canine for about a year now. It started when I got tired of the overhead and high costs of hosting my web apps on services like Heroku, Render, Fly.io, and others. At one point, I was paying over $400 a month for cloud hosting. Last year, I switched everything over to Hetzner.

### Cost comparison for a 4GB server:

- **Heroku:** $260  
- **Fly.io:** $65  
- **Render:** $85  
- **Hetzner:** $4  

*(Costs increase significantly when more than 4GB are needed.)*

The main downside of using Hetzner is that it doesn’t offer a very straightforward way to handle tasks like:

- DNS and SSL certificate management  
- Team management  
- GitHub integration  

However, I believed it would be simple enough to build a lightweight platform similar to Heroku for my Hetzner instance. It turned out to be more challenging than I expected, but after a year, I've made good progress.

### Key features of Canine

The best part is that it makes hosting any Helm chart trivial. This opens up a wide range of open-source projects—everything from databases like Postgres and Redis to various other services, such as torrent trackers or VPN endpoints.

### Find out more

- **Open source:** [https://github.com/czhu12/canine](https://github.com/czhu12/canine)  
- **Cloud hosted version:** [https://canine.sh](https://canine.sh) (nofollow)