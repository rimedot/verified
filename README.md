# Meva verified plugins

The signed list of plugin versions Meva treats as verified, and the audit
note for each one.

- `verified-list.json`: the signed list Meva reads (DSSE envelope, Ed25519,
  key id `6be24bbeaa157aff`). Meva fetches it from
  `https://raw.githubusercontent.com/rimedot/verified/main/verified-list.json`,
  checks the signature, refuses an older or expired list, and turns off
  versions listed under `revoked`.
- `list.json`: the unsigned list it was signed from.
- `audits/`: what was checked for each listed version.

A version is listed when its release file matches the hash here, its GitHub
build attestation verifies, and its audit note is in `audits/`.
