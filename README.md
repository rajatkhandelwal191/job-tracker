# Encrypted Job Search Pipeline Tracker

This repository hosts a client-side encrypted static build of Rajat Khandelwal's Job Search Automation Dashboard.

- **Encryption**: AES-256-GCM authenticated encryption.
- **Key Derivation**: PBKDF2 with SHA-256 (100,000 iterations) derived client-side in the browser via `window.crypto.subtle`.
- **Privacy**: The underlying job search data, company names, notes, and fit scores are 100% encrypted ciphertext in storage and are decrypted strictly in memory upon PIN entry.
- **Hosted on**: GitHub Pages via GitHub Actions.
