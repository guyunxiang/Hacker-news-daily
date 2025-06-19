# Show HN: Unregistry – "docker push" directly to servers without a registry

**Posted by psviderski on 2025-06-18**

I got tired of the push-to-registry and pull-from-registry dance every time I needed to deploy a Docker image.

In some cases, using a full-fledged external or even local registry can be unnecessary overhead. After all, there’s already a form of registry present on any Docker-enabled host — Docker’s own image storage.

So I built Unregistry [1], which exposes Docker’s (containerd) image storage via a standard registry API. It introduces a `docker pussh` command that pushes images directly to remote Docker daemons over SSH. The transfer is efficient, sending only the missing layers, making it fast.

Here's how it works:

```bash
docker pussh myapp:latest user@server
```

Under the hood, it launches a temporary Unregistry container on the remote host, pushes the image through an SSH tunnel, and cleans up afterward.

I developed this while working on Uncloud [2], a tool for deploying containers across a network of Docker hosts. I thought it might be useful as a standalone project.

Would love to hear your thoughts and potential use cases!

---

**Links:**

- [Unregistry on GitHub](https://github.com/psviderski/unregistry)
- [Uncloud on GitHub](https://github.com/psviderski/uncloud)