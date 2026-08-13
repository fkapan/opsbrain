# OpsBrain Desktop — Private Beta

OpsBrain is a local-first Windows desktop assistant for system and platform engineers. It is designed for Kubernetes, OpenShift, Linux, Java applications, PostgreSQL, Oracle, Redis, RabbitMQ, SAS Viya, SAS 9.4 and related enterprise operations work.

This repository is a **binary distribution and feedback channel only**. The OpsBrain source code is intentionally private during the beta period. The project may become open source after the beta program is complete.

## Download

Open the latest GitHub Release and download:

- `OpsBrain-Setup-1.0.0-beta.2.exe`

The Portable build is not part of this public beta distribution.

## Interface preview

These promotional collages use real OpsBrain beta screens:

![OpsBrain operations cockpit](./assets/opsbrain-collage-operations-cockpit.png)

![Vault, files and knowledge](./assets/opsbrain-collage-vault-files-knowledge.png)

![Context, health and environments](./assets/opsbrain-collage-context-health.png)

## System requirements

- Windows 11 64-bit
- Recommended: Intel Arc A770 16 GB, AMD Ryzen 9 7900X, 64 GB RAM
- A local GGUF model and llama.cpp runtime configured by the user
- Approximately 1 GB free disk space for the application package, plus model storage

The recommended hardware is not a guarantee of model speed. Model size, quantization, context size and GPU driver state affect performance.

## Privacy and safety

- Inference is local through llama.cpp on `127.0.0.1`.
- No cloud AI API, telemetry, SSH, kubectl/oc, PowerShell, SQL or automatic command execution is included.
- Commands suggested by the assistant are display-only and classified as GREEN, YELLOW or RED for review.
- Customer folders, conversations, logs and credentials remain local to the Windows user profile.
- Do not upload customer logs, credentials, tokens, private keys or other confidential operational data to public GitHub Issues.

## Beta limitations

- This is a pre-release build and may contain defects.
- PDF/DOCX content parsing, TOTP, password history and live infrastructure connectivity are limited or unavailable.
- The local llama.cpp model and model files are not included in this download.
- Source code is not distributed during the beta.

## Verify the installer

In PowerShell, after downloading the installer and `SHA256SUMS.txt`:

```powershell
Get-FileHash .\OpsBrain-Setup-1.0.0-beta.2.exe -Algorithm SHA256
Get-Content .\SHA256SUMS.txt
```

The calculated hash must match the value in `SHA256SUMS.txt`.

## Feedback

Please use GitHub Issues for reproducible bugs and product feedback. Include:

1. OpsBrain version and Windows version
2. CPU/GPU/RAM and CPU/GPU mode
3. The page or workflow where the problem occurred
4. Safe reproduction steps
5. Expected and actual behavior
6. A screenshot or redacted log when useful

Never include passwords, tokens, private keys, kubeconfig files, connection strings or unredacted customer data.

For direct contact, replace the placeholders in `RELEASE-NOTES.md` with the maintainer's preferred GitHub username or email address before publishing the repository.

## License status

The beta executable is distributed for evaluation and feedback. It is not an open-source release. See `LICENSE-NOTICE.md`.
