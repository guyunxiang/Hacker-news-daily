# Show HN: Tlsinfo.me – check your JA3/JA4 TLS fingerprints

**Posted by elpy1 on 2025-07-16**

Recently, I was learning about TLS and found myself capturing network traffic with `tshark`, then opening Wireshark to import the dumps and check fingerprints. To make this process easier, I created a simple service for quick TLS fingerprint checks.

You can curl [https://tlsinfo.me/json](https://tlsinfo.me/json) or visit the site directly from your browser. It returns the TLS fingerprint presented by your request, including:

- JA3
- JA3 raw
- JA4
- JA4 raw

There’s no authentication required, and QUIC support is included. To prevent abuse, the service is rate-limited to 10 requests per 10 seconds per IP—please be considerate.

This tool could be handy for:

- Learning about TLS fingerprints
- Debugging network issues
- Investigating how different clients or software leave distinct fingerprints
- Adding simple fingerprint checks into scripts or automation pipelines
- Setting up a reverse proxy or custom domain on Cloudflare CNAME pointing to tlsinfo.me for fingerprint verification

Let me know if you find it useful! Feel free to reach out with questions or ideas. Thanks!