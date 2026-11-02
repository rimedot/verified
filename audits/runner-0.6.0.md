# runner 0.6.0 — audit

- Date: 2026-11-02
- Release: https://github.com/rimedot/runner/releases/tag/v0.6.0
- Files and sha256: runner.mevax f05d8d11ed56e43752abd7b9dcaca94bc3bf9d0222891fc2d30f6c75d6e7aacb, runner-linux-x86_64.tar.gz 8bbbb2944d009caed2d65bef5bd1e303af4cff4df01c72372a29496a13807ed9
- Build attestation: verified with `gh attestation verify --repo rimedot/runner` (built by this repo's release workflow).
- What was checked: the source was scanned for keys, tokens, personal paths and private hosts before publishing (none found); the binary is built from this repo by its release workflow; the manifest declares GPU use and network to github.com, objects.githubusercontent.com, release-assets.githubusercontent.com and files.pythonhosted.org (runtime pack downloads, each pinned by sha256); its tests pass (98); MIT.
- Not checked: a full security review of the Rust source; remote worker setup also contacts ghcr.io and a pairing broker, which the manifest does not list.
