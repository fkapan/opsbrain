# OpsBrain 1.0.0-beta.2 — GitHub Release Text

Use the following content as the GitHub Release title and description.

## Suggested title

`OpsBrain 1.0.0-beta.2 — Windows Private Beta`

## Suggested tag

`v1.0.0-beta.2`

## Release description

OpsBrain 1.0.0-beta.2 is a **Windows-only private beta** for system and platform engineers.

This release focuses on:

- Local llama.cpp inference
- Turkish and English operation
- Long-conversation performance profiles: Fast, Balanced and Deep Analysis
- Customer and environment context
- Encrypted local Credential Vault
- Managed File Manager with preview, metadata and local AI analysis
- Display-only command intelligence with GREEN / YELLOW / RED risk levels
- Kubernetes, OpenShift, Linux, Java, PostgreSQL, Oracle, Redis, RabbitMQ and SAS operations workflows

### Important safety notice

OpsBrain does not automatically execute shell, PowerShell, kubectl, oc, SQL or destructive commands. It does not connect to customer infrastructure. Suggested commands must be reviewed and run manually by an authorized engineer outside the application.

### Included asset

- `OpsBrain-Setup-1.0.0-beta.2.exe`

Portable builds and source code are intentionally not included in this public beta release.

### Known limitations

- Local llama.cpp and GGUF model setup is required; models are not included.
- Live infrastructure access is not implemented.
- PDF/DOCX parsing, TOTP and password history are limited or unavailable in this beta.
- Performance depends on model size, quantization, context size and hardware drivers.

### Feedback requested

Please test the installer and report:

- Installation or launch problems
- Local model/runtime problems
- Turkish/English language issues
- Conversation persistence or long-history issues
- Credential Vault or File Manager usability issues
- Incorrect command risk classification
- Health Check and domain workflow gaps

Please redact all customer names, hostnames, IP addresses, credentials, tokens, private keys, kubeconfigs and confidential logs before posting.

### Maintainer contact

Replace these placeholders before publishing:

- GitHub: `@[MAINTAINER_GITHUB_USERNAME]`
- Email: `[MAINTAINER_EMAIL]`

GitHub Issues are preferred for non-sensitive beta feedback. Use the maintainer's private contact for security reports.

### Verification

The installer SHA-256 is published in `SHA256SUMS.txt`. Verify it in PowerShell with:

```powershell
Get-FileHash .\OpsBrain-Setup-1.0.0-beta.2.exe -Algorithm SHA256
```

The expected value for this build is:

```text
834C28875AADA45E7173C82716AA5156DDCCC428718DCDB4B07D1A22775BAED4
```

This is a beta evaluation build. Please do not use it as a substitute for change management, peer review, backup or operational approval.
