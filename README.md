# Cold Case #011 — Exoplanet periods lean the same digit-direction in every survey

Site card: https://projectaletheia.org/cold-cases#cc-011
Hub: https://github.com/0100001001101111/aletheia-cold-cases

## The case in one breath

The orbital periods of ~6,000 vetted exoplanets depart from Benford's
first-digit law — overall, in transit surveys, and in radial velocity —
and the departures lean the SAME direction in each independent detection
method. The favored explanation is survey selection (which orbits each
telescope can detect), but that explanation cannot currently be tested:
it needs per-facility detection-probability models that mostly are not
public. Until then the same-direction lean is measured, replicated, and
unexplained at the control level.

Ceiling: descriptive. This is a question and a data request, not a
finding. The underlying run refused to promote the raw departure as a
finding precisely because it could not pass selection controls.

## What we need

Survey completeness / detection-probability models — detection
probability as a function of orbital period, per facility — from the
Kepler, TESS, and radial-velocity teams. Published or shareable. With
any such model in hand, the frozen digit test re-runs conditioned on it
and the case closes in either direction.

## What's here

- `CASE_FILE.md` — the cold-case record (plain words, ceiling, ask)
- `REPORT.md` — the full run write-up: frozen design, 200,000-draw tests
  with Holm correction, the control suite, what failed and why
- `POSTABILITY.md` — the run's own refusal to promote the finding
- `receipts/` — frozen manifest with SHA-256 hashes, novelty audit,
  verified run closeout

No NASA Exoplanet Archive data is redistributed here; the archive is
public and the frozen manifest pins the exact snapshot by hash.

Contact: bo@projectaletheia.org
