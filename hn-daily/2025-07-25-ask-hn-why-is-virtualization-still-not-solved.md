# Ask HN: Why is virtualization still not solved?  
**Posted by prmph on 2025-07-25**

It's 2025, and virtualization remains a headache, even for casual use.

I use a MacBook Air M1 as my dev laptop, and I wanted a reproducible Debian development environment. My options were either using devcontainer or running a full VM with VirtualBox, VMware, Parallels, UTM, etc.

**Challenges I faced:**

- **VSCode & TypeScript issues:** They occasionally break, making development impossible. I suspect internal bugs that surface under specific conditions. Since devcontainer runs VSCode directly on my machine connecting to a container, it’s not a true VM solution, and I need a real VM.

- **VirtualBox:** After hours of installing Debian and getting the VM running smoothly, performance quickly degraded, slowing to a crawl. Display resolution issues persisted. I gave up, again—every few years I try this and forget why I stopped.

- **VMware:** Tried to evaluate it after noticing it was sold to Broadcom. Downloading is problematic—it requires login, and there’s no easy registration process.

- **Parallels:** Finally, I got a Debian VM running smoothly and was willing to pay for a good experience. However, after some time, I encountered random internet connectivity drops (affecting only the terminal). Changing networking modes (shared to bridged) and adjusting firewalls didn’t resolve the issue; in fact, connectivity worsened. It reminded me why I didn’t want a Parallels subscription in the first place.

Frustrated, I gave up again. I also remember that UTM shares similar performance and display issues as VirtualBox.

**What options are left?**  
Installing dual-boot Linux on a Mac is not straightforward—especially on Apple Silicon (Asahi aside), since I only want Debian. Alternatives include using a cloud VPS or purchasing new AMD mini PCs to run Debian. But ultimately, after decades of supposed technological progress, virtualization still feels unresolved and problematic.