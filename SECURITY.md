# Security / الأمان

If you find a security problem in WorkBase (for example a way to read vault secrets without authentication, or data leaving the Mac unexpectedly), **please don't open a public issue.** Email **mohamed.kh.hamad@icloud.com** with:

- what you found and its impact,
- steps to reproduce,
- your WorkBase and macOS versions.

We'll reply as soon as we can. Please give us a reasonable time to ship a fix before sharing details publicly.

إذا وجدت مشكلة أمنية في WorkBase فمن فضلك **لا تفتح بلاغًا عامًا**، وراسلنا على البريد أعلاه مع التفاصيل وخطوات التكرار.

## How WorkBase protects data
- Data is stored locally; there is no WorkBase server or account.
- Vault secrets live in the macOS Keychain and are shown only after Touch ID or the Mac password.
- The only outgoing requests are the website/SSL checks you configure.
- Encrypted backups use AES-256-GCM with a key derived from your password (PBKDF2-SHA256).
