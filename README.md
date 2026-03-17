# dextech.onoma.lib.policy

Public distribution repo for the sealed Onoma naming-policy artifact.

This repo is consumed by:

- `dextech.onoma.app/apps/client`
- bundled operator tooling
- server/bootstrap applications that need current naming suggestions

It should contain only generated public distribution artifacts. The human
canon lives elsewhere and is not committed here.

## Canonical Source

The source canon remains in:

- `dex.spec.core/docs/repo-naming-and-token-taxonomy-v2.4.2.md`

The admin Onoma app reads that canon, extracts the machine-readable appendix,
encrypts it to a recipient certificate, signs it, and publishes the sealed
artifact into this repo.

## Expected Artifact Path

- `policy/onoma-policy.sealed.json`
