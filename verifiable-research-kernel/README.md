# IntentSeal Verifiable Research Kernel (VRK)

## Current release — v0.3.1

Artifact: `IntentSeal_Verifiable_Research_Kernel_v0_3_1.zip`

SHA-256:

`c18c4c697d8188490e96530cfb5ddcb2e63f7c65aa560415401b1541e575cd79`

Size: **177,783 bytes**  
ZIP entries: **89**  
Checksum-manifest entries: **88**

Deterministic certificate digest:

`09209816a034020076e0f66e1b8924b6dd1567c95f7159070f58ce62ac597a8f`

### Demonstrator 001 — finite LRSC

- state: **CERTIFIED**
- K0..K13 exact coverage: **527,046,644,056**
- K13 search nodes: **3,432**
- K14 integer interval witness: PASS
- tests: **30/30 PASS**
- adversarial cases: **33/33 rejected**
- promotion: **EVIDENCE_BOUND -> CERTIFIED**
- certificate-bound dual seal: PASS

Verifier-source trust root digest:

`f010a99d78b360b8fd5dc9b727f21b898889c6e75e3093cc22d6f04d005a0d0f`

Public anchor commit:

`e3b43046346c91faf2333d18d50c87012c8b162a`

### Demonstrator 002 — finite N11 K36 crossing

Scientific certificate archive SHA-256:

`d29224e1dd4ad9f9454951415a3b080bc9f092839e24caaeddd056013785cfbe`

Final package check: PASS.

VRK state: **EVIDENCE_BOUND**.

That lower state is deliberate because v0.3.1 does not independently regenerate all 120 Arb enclosures. It verifies the frozen package and theorem gates without silently inheriting the external project's stronger interval-certification status.

See [the final release audit](VRK_v0_3_1_FINAL_2026_09_28.md).

## Historical baseline

v0.3.0 remains immutable:

`b01178e81b0e0f07c67a883d8e51430f8af0dc608c5246ee925f6c5c17c0b52c`

The scientific proposition identity for Demonstrator 001 is unchanged across the evidence promotion.

## Boundary

Evidence certification and IntentSeal publication authority remain separate. The included authority seal is a symmetric HMAC demonstration, not production authorization infrastructure.

Neither demonstrator establishes any continuum Navier–Stokes theorem or universal physical claim.

No VRK DOI is claimed yet.
