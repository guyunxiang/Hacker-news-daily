# Show HN: I built a cloud on my own ASN with real 1:1 compute to fight the cartels

**Posted by ccheshirecat on 2025-06-25**

---

I'm MX, a solo founder building Infuze Cloud, launching as a beta today.

I started this project because I was tired of numerous reasons why the cartels are ridiculous—reasons I won't dwell on here. Honestly, I had to rewrite this twice due to hitting character limits. So I decided to build something I'd actually want to use.

The entire stack is built custom from scratch, with no external dependencies or third-party costs—only hardware and IP space.

## What is Infuze?

- **Raw, dedicated performance:** 1 vCPU = 1 physical thread. No overcommitment. Node allocations are capped at the hardware limit with some overhead.
- **Pricing based on usage:** It’s set at $10/month for 4GB RAM / 1 vCPU / 50GB storage, with provisioning in 1-hour blocks (approx. 3 cents). Wallet top-ups offer discounts to prevent pressure to over-provision. Even the minimum top-up starts at a 10% discount (~$8/month), dropping to ~$7.50 with larger top-ups.
- **Own hardware and autonomous system:** Operating leased Intel Xeon Platinum 8280 servers with BGP-routed IP space (AS211747).
- **Storage:** NVMe Gen4 with ZFS.
  
## The Stack

Built primarily on open-source technology:

- **Virtualization:** Proxmox
- **Networking:** Knot DNS as master, outsourced anycast slaves, using FRR for BGP.
- **Routing:** Standard bridged networking routed from leased IP space announced via FRR.
- **Storage:** NVMe Gen4 with ZFS
- **Microservices:** Custom Go-based for frontend automation (some will be open-sourced soon)
- **Mail:** Maddy
- **Metrics & Monitoring:** Prometheus, Node Exporter, Grafana
- **LLM Chatbot:** Using AnythingLLM with OpenRouter (more a FOMO experiment—I don’t expect heavy use)
- **Support/Tickets:** Custom system with Next.js frontend
- **Billing:** Stripe
- **Networking for VMs:** Each VM gets a public IPv4 and a /64 routed subnet (no NAT or SNAT)

If you’re curious about any part of the stack or want to discuss optimizations, I’m very open. I’m still learning as I go. I also have plans for something more experimental: a custom Firecracker fork that boots ELF+IVSHMEM apps directly from memory with a unikernel or initramfs. I hope to share that soon, but funding has been tight.

## Who is this for?

- Developers who prefer Linux with root access, via SSH, etc.
- Those who want infrastructure close to real costs—compute isn’t expensive, and the tech isn’t overly complicated. We shouldn’t be paying a monopoly’s premium.
- Not for yaml-therapy fans or those who love contributing to charitable foundations with wooden figureheads—though I’ve got something lined up for you too! 😉

This is the first public beta. While most components are battle-tested, expect a few bumps. I’ll be around today to answer questions, fix bugs quickly, and learn from your feedback.

## Benchmark Site

For the tech enthusiasts, I set up a fun quick site with version 0.0 because I kept tinkering and delaying launch out of impostor syndrome. Check it out:

[https://bench.infuze.cloud](https://bench.infuze.cloud)

You can get a free dollar voucher there and run a benchmark for fun. I wanted to do larger tests but real-time billing could invite abuse, and being self-funded, I need to be cautious. I’m ready to pivot if needed and strike back against bad actors. 😉

Thanks for reading! I’d love to hear your feedback, ideas, or critiques. Appreciate you all.