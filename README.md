# Interview season

Password-protected, mobile-friendly interview tracker. The tracker and its initial program data are encrypted with AES-256-GCM and a PBKDF2-SHA256 password-derived key. Only the unlock screen and encrypted payload are public.

Keep me signed in remembers the decryption key in this browser until Lock is selected or website data is cleared. Progress is encrypted locally and synced to the shared storage service. Offline edits are queued on the device and uploaded after reconnecting. Backup files and CSV exports contain readable progress; keep them private. Browser storage is not guaranteed to survive clearing data or private browsing.

Frontend deployment: GitHub Pages, main branch, root folder. Shared encrypted progress is stored in the Interview Tracker Sync service. HTTPS is required for browser cryptography.
