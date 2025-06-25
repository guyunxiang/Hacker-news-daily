# Show HN: VSCan - Detect Malicious VSCode Extensions

**Posted by shadow-ninja on 2025-06-24**

Did you know that VSCode extensions run with full access to your system—including the file system, network, and credentials? Worryingly, dozens of malicious extensions have already made it into the marketplace, silently compromising devices.

As a security researcher and student developer, I encountered this problem firsthand. To address it, I built VSCan—a completely free tool (no login required)—that scans VSCode and Cursor/Windsurf extensions for:

- Hidden malware and obfuscated code  
- Dangerous permissions and API misuse  
- Vulnerable dependencies and suspicious network connections  

Users have already uncovered hundreds of vulnerabilities in extensions. VSCan produces a clear, developer-friendly security report to help you understand what you're installing.

Try it out: [https://www.vscan.dev](https://www.vscan.dev)

Additionally, I have developed a custom sandboxing security architecture to restrict extensions from malicious activity during runtime. This technology is unique, and if you're interested in testing it or learning more, please reach out!

Your feedback would be greatly appreciated. Thanks for your support!

---

## Insights from a Sample of 1077 Marketplace Extensions

- 3 extensions are marked as malicious by VirusTotal  
- 7 extensions use malicious network connections (verified by VirusTotal)  
- 33 extensions have dependencies with critical vulnerabilities  
- 39 extensions contain sensitive information such as API keys, usernames, or passwords  
- 204 extensions display poor development practices, as flagged by OSSF  
- 71 extensions request very high permissions (not necessarily malicious but a potential red flag)  

### Example Analysis
Here is a link to an extension with malicious network endpoints:
[https://vscan.dev/?analysisId=9e6c1849-3973-402b-a4ff-3b4023508fb8](https://vscan.dev/?analysisId=9e6c1849-3973-402b-a4ff-3b4023508fb8)