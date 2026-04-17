# SendCipher – End-to-end encrypted file sharing

**Only you, and the recipient you share the password with, can access the file. The server sees only encrypted data.**

## How it works

- A single **Rust library** is compiled to **WebAssembly** (for the browser) and used natively by the **CLI**
- Files are cut into **chunks**, each encrypted with **AES‑256‑GCM**
- **Encryption and upload are performed in parallel** (Web Workers in browser, threads in CLI)
- The server **never stores file names** – they are part of the encrypted metadata

## Built from scratch

By a **single developer** in about **4 months** (Sept 2025 – Apr 2026).  
Privacy and encryption were the core features from **day 0**, not added later.

---

🔗 **[Website](https://sendcipher.com)** · **[Repository](https://github.com/youcefl/sendcipher)**
