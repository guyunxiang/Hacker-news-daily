# Show HN: Zkshare – PIN protected secret sharing with client-side encryption

**Posted by streetsmartai on 2025-07-29**

I built zkshare to enable secure secret sharing without trusting the server.

### Features
- Client-side encryption secured with a 6-digit PIN
- The server never sees secrets in plaintext
- Wrong PIN attempts do not compromise the secrets
- Single-use tokens that self-destruct after decryption
- Python CLI for managing `.env` files and a React web app interface

### Tech Stack
- Rust backend (Axum + Redis)
- React frontend
- Python CLI

### Try it out
```bash
git clone https://github.com/streetsmart-ai/zkshare.git
cd zkshare/backend && cargo run
cd ../zkdotenv && python3 test_zkcloud_encrypt.py
```

This project is open source and MIT licensed. I’d love to hear feedback on the security model!