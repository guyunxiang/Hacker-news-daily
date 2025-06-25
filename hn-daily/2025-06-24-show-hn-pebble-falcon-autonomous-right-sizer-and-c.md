# Show HN: Pebble Falcon – Autonomous Right-Sizer and Carbon-Aware Kubernetes Scheduler

**Posted by kevalshah90 on 2025-06-24**

Hi HN — I’m Keval, part of the AI team behind Pebble Falcon.

## What is Pebble Falcon?

Pebble Falcon consists of two long-running agents you deploy inside your Kubernetes cluster:

### PerfectFit
- Streams pod, VM, and GPU utilization
- Calculates available headroom
- Generates JSON patches to right-size CPU, memory, and storage
- Includes an optional human approval step

### EcoAgent
- Polls real-time grid carbon intensity data
- Reconfigures GPU nodes and pods to maximize clean energy usage
- Re-queues batch jobs to regions with the lowest gCO₂/kWh that still meet your latency SLAs

A lightweight web UI displays the cost savings, watts avoided, and provides a 30-day projection.

**Security Note:** No data leaves the cluster; the only inbound feed is the public carbon intensity data.

## Why We Built It

We noticed GPU nodes often idled below 20% while ETL jobs ran in high-carbon regions. Manual rightsizing sprints couldn't keep up with this inefficiency.

**Pilot Results (40-node GPU cluster over 30 days):**  
- 70% of idle compute was removed  
- 4,160 kg of CO₂ avoided (equivalent to about six NYC→London flights)

Pebble Falcon requires access to your clusters, so there's no public sandbox yet. Instead, we've recorded a 3-minute overview of the agents:

[Video Demo](https://youtu.be/DTpHxAmVrAo)

If you're interested in trying it out, comment below and we'll get in touch. We can also add you to our pilot program: [Sign up here](https://www.gopebble.com/sign-up).

---

Feel free to AMA about energy-aware, cost-effective, and compute-aware scheduling for AI workloads!