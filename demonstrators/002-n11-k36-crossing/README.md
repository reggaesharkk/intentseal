# Demonstrator 002 — finite N11 K36 crossing certificate

This demonstrator records a different evidence architecture from LRSC: a computer-assisted validated trajectory for one explicit finite-dimensional Fourier-Galerkin ODE.

## Certified proposition

For the fixed finite N11 Fourier-Galerkin trajectory at viscosity (
u=0.1), starting from the exact rationally interpreted 112-pair witness used by the Navier–Stokes Bridge Audit, the frozen K36 observable (F=I-9O) has nonzero normalizer on ([0,0.003]) and there exists at least one (t_*\in(0,0.003)) such that (F(u(t_*))=0).

## Certificate identity

- archive: `N11_K36_Turnover_Certificate_2026-09-28.zip`
- SHA-256: `d29224e1dd4ad9f9454951415a3b080bc9f092839e24caaeddd056013785cfbe`
- archive entries: 257
- whole-segment Arb enclosures: 120 / 120
- protocol: `wp16-n11-arb-hermite-v1-exact-rational-start`
- precision: 128 bits

Certified bounds:

| Gate | Outward bound |
|---|---:|
| (F(u(0))) | ([645.8037741471,645.8037741472]) |
| final trajectory error | (<0.00004588841) |
| uniform normalizer | (>48990.29795521) |
| (F(u(0.003))) | ([-54.748409847,-42.032667894]) |

A separate exact-Fraction/Taylor recurrence gives error (<0.000045868444), below the padded Arb radius used in the endpoint proof.

## Scope

The datum was selected post hoc. The result is a theorem for **one fixed finite N11 Galerkin trajectory**. It does not prove continuum Navier–Stokes regularity, blowup, all-cutoff persistence, or a Millennium-problem result.

Canonical repository: https://github.com/reggaesharkk/navier-stokes-bridge-audit
