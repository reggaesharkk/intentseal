# IntentSeal Verifiable Research Kernel

VRK is the scientific-claim verification layer inside IntentSeal. It treats scientific claims as typed objects with explicit proposition identity, evidence bindings, dependencies, verifier outputs, scope boundaries, and promotion state.

## Current release state

### v0.3.0 — frozen historical baseline

Artifact SHA-256:

`b01178e81b0e0f07c67a883d8e51430f8af0dc608c5246ee925f6c5c17c0b52c`

Demonstrator 001 finite LRSC result:

- K0..K13 exact coverage: 527,046,644,056 / 527,046,644,056
- K13 search nodes under proof-preserving channel permutation: 3,432
- K14 direct interval witness: PASS
- tests: 22/22 PASS
- adversarial mutations: 13/13 rejected

Kernel identities:

- proposition digest: `c8e24478afe2579f25020ded46f93e379b414caf4dc466f45e0dac0a854ec0cf`
- claim digest: `78f86c4935699ff78ec658ba4856804b74908e5b23d83ef39b11cf592d241296`
- evidence root: `5822eba24c030bf6005a414a19d75e7c5836f489349d7954ec25a192f65b50f9`
- dependency root: `d067270a3a25b60d39fe9fa7185f77d1cb6d038e7925062325f00c4a8a6b4738`

### v0.3.1 — candidate only

Candidate SHA-256:

`5ab780860ac1f7629e51ecaacff4ed0003b34909eea6ef47815f7d27a2d47ba5`

Deterministic certificate digest:

`b0e58b19a4830e8ad4f9d5dbad0d1d354a4e7ce02ed9b7ca5ada05f6e1ba0a62`

The candidate is **not final**. Open gates include the expanded adversarial suite, certificate-bound promotion and authority receipts, and an external trust anchor for all verifier sources.

## Evidence versus authority

VRK evidence certification and IntentSeal action/publication authority are intentionally separate. A stronger epistemic label cannot be obtained merely by possessing an authority receipt, and a scientific certificate does not grant privileged execution authority.

## Scope

A VRK `CERTIFIED` state means that the stated finite-domain verifier accepted the required evidence package under the declared semantics. It is not peer review and not a universal truth claim.
