# GitHub-only binary distribution checklist

## Recommended repository

Create a separate public repository, for example:

`OpsBrain-Beta`

Keep the application source repository private. This public repository should contain only the files in this folder plus the GitHub Release assets.

## Before publishing

- [ ] Replace maintainer username, email and private security contact placeholders.
- [ ] Create the public repository with no source-code files.
- [ ] Add `README.md`, `LICENSE-NOTICE.md`, `SECURITY.md`, `RELEASE-NOTES.md` and `FEEDBACK-TEMPLATE.md`.
- [ ] Create a GitHub Release tagged `v1.0.0-beta.2`.
- [ ] Upload only `OpsBrain-Setup-1.0.0-beta.2.exe` and `SHA256SUMS.txt`.
- [ ] Do not upload the source repository, `src/`, `electron/`, `node_modules/`, `.artifacts/`, `.backups/`, model files, customer data or private logs.
- [ ] Do not upload `OpsBrain-Portable-1.0.0-beta.2.exe` if the public beta is Setup-only.
- [ ] Mark the release as a pre-release.
- [ ] Verify the published asset hash after upload.

## GitHub UI steps

1. Create the empty `OpsBrain-Beta` repository.
2. Add the public documentation files.
3. Open **Releases → Draft a new release**.
4. Set tag `v1.0.0-beta.2` and enable **Set as a pre-release**.
5. Paste `RELEASE-NOTES.md` into the description.
6. Attach the Setup executable and `SHA256SUMS.txt`.
7. Publish the release.

GitHub release assets can be large, but the repository itself should remain documentation-only. Do not commit the installer into normal Git history.
