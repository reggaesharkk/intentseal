# IntentSeal / VRK release audit — 28 September 2026

## Frozen reference artifacts

- VRK v0.3.0 source ZIP SHA-256: `b01178e81b0e0f07c67a883d8e51430f8af0dc608c5246ee925f6c5c17c0b52c` (matched). Its 72-entry checksum manifest matched on the pristine extraction; 22 tests passed; fresh LRSC replay and post-run verifier passed.
- Foundational IntentSeal lineage archive SHA-256: `05ba923c90dfc481a70a3784b72d1cd71a0adeac2c34a22631169f545ae5d4c0`, 161324 bytes. ZIP CRC check passed. Five inner release SHA-256 values match the outer release manifest. Its outer LICENSE is All Rights Reserved.

## v0.3.1 candidate

Candidate ZIP: `IntentSeal_Verifiable_Research_Kernel_v0_3_1_CANDIDATE.zip`  
SHA-256: `5ab780860ac1f7629e51ecaacff4ed0003b34909eea6ef47815f7d27a2d47ba5`  
Size: 146950 bytes. 73 manifest entries.

Two clean-room source runs and one freshly extracted ZIP run returned identical canonical certificate digest:

`b0e58b19a4830e8ad4f9d5dbad0d1d354a4e7ce02ed9b7ca5ada05f6e1ba0a62`

Each run regenerated LRSC inputs, compiled the bundled C++ search, independently post-checked the result, and ran 22 existing tests. K0–K13 coverage was `527046644056`, K13 search nodes `3432`; K14 integer interval inequality passed.

## Release blockers and trust boundary

The new certificate runner binds source hashes and generated proof inputs but imports claim identity fields from the packaged v0.3.0 receipt. The certificate and manifest can both be resealed by someone who rewrites non-vendored verifier source. The requested broader adversarial suite, certificate-bound promotion receipt, and certificate-bound authority dual seal were not completed in this candidate. Hence this is a **candidate**, not a final release.

## Publication status

No DOI is claimed for either archive in this dated audit. The foundational archive is ready for a Zenodo draft when authenticated access is available; the VRK candidate is not ready for deposit.
