# Benford first digits in confirmed exoplanet periods

No action needed. The BENFORD-PERIODS run finished as a non-novel informative null under the full frozen selection-control rule.

**The plan:** Bo asked whether confirmed exoplanet periods follow Benford's first-digit distribution overall and by four discovery methods, and whether any departure survives selection controls.

**What I did:** I froze the archive query and tests, saved both NASA tables, checked five branches, ran the full control suite, replayed the result independently, audited prior work, and obtained Grok review.

## The investigation from the beginning

1. 🧾 **The original claim**

   The question came from Bo's BENFORD-PERIODS goal at The question. The goal asked whether confirmed exoplanet orbital periods follow Benford's first-digit pattern, whether the result differs across four discovery methods, and whether any departure survives controls for how planets enter the archive.

   A robust first-digit departure could expose a useful survey fingerprint or a data-integrity warning. A clean null would show where a simple digit test stops being informative.

2. ⚠ **The suspected crack**

   A stable digit pattern can come from which periods surveys can detect and confirm, from the finite measured range, from the mix of eras and facilities, or from repeated planets around one host.

3. ✅ **The planned test**

   I counted exact decimal first digits, used 200,000-draw tests with Holm correction and a practical effect floor, then checked units, complete windows, eras, facilities, host clustering, a second archive table, and cross-era smooth period models.

   The claim would look stronger only under this result. An adequately sized branch rejects the Benford reference and keeps that result across every frozen unit, window, era, facility, host, table, and smooth-selection control. This outcome would mean the saved archive snapshot has a first-digit departure that the named selection and representation checks do not explain.

   The crack would look stronger only under this result. A raw departure loses statistical or practical support under any load-bearing selection or representation control in the frozen rule. This outcome would mean the raw digit pattern cannot support an intrinsic population, method, or archive-integrity claim in this run.

   The test would be unclear under this result. The data cannot be acquired, the verifier fails planted known answers, or the named branch lacks enough rows for the frozen inference rule. This outcome would mean the available run cannot settle that branch and must remain blocked or descriptive instead of being called conforming.

4. 🧾 **What happened**

   The raw test rejected Benford overall in 6,003 periods, in 4,688 Transit periods, and in 1,195 Radial Velocity periods. No branch passed the full frozen selection-control rule. Imaging had 26 rows and Microlensing had 12.

   A small raw p-value was not enough. The measured-range and selection-matched null removed the practical departure or the statistical departure, so the raw pattern cannot carry the stronger claim.

5. ⚠ **Still unresolved**

   This run cannot name the cause of the digit shape. A causal test needs an external survey-completeness model or a prospective prediction on archive rows that did not train the model.

## The exact result

- Overall: 6,003 eligible periods. The raw first-digit counts were 1,658, 990, 876, 677, 526, 389, 302, 318, and 267. The Holm-adjusted Monte Carlo p-value was 0.000024999875000624998. Total variation was 0.04711783171372501.
- Transit: 4,688 periods. The raw counts were 1,294, 774, 694, 532, 395, 293, 245, 247, and 214. The adjusted p-value was 0.000024999875000624998. Total variation was 0.04628164571116315.
- Radial Velocity: 1,195 periods. The raw counts were 341, 191, 159, 129, 122, 91, 52, 62, and 48. The adjusted p-value was 0.03749981250093749. Total variation was 0.05200039937099506.
- Imaging had 26 periods. Microlensing had 12. Both stayed descriptive under the frozen minimum of 50.
- At the main cross-era smooth bandwidth of 0.15 log10 days, Overall had adjusted p=0.03129937401251975 but total variation 0.025426065306289443, below the 0.03 practical floor. Transit had adjusted p=0.1115177696446071. Radial Velocity had adjusted p=0.7188456230875382.
- The discovery-method comparison had conditional permutation p=1.0 after fixed log-decade and discovery-era stratification.
- The PS replay matched all 5,989 common eligible periods exactly. It is dependent robustness evidence because it shares the archive and discovery process.

## What it's NOT ⚠

- This is not proof of Benford conformity, because Overall, Transit, and Radial Velocity reject the raw reference.
- This is not proof that selection caused the pattern, because the smooth null describes the measured range but cannot identify a causal survey process.
- This is not an archive-error finding, because a first-digit distribution does not identify a bad row.
- This is not a discovery-method effect, because the controlled method permutation returned p=1.0.
- This is not evidence about Imaging or Microlensing conformity, because their samples were below the frozen inferential minimum.

## Receipts 🧾

- Frozen recovery manifest: `01_prereg/FROZEN_IMPLEMENTATION_RECOVERY_MANIFEST_V5.json`
- Saved NASA data: `02_data/target_snapshot_v1/pscomppars.csv` and `02_data/target_snapshot_v1/ps_default.csv`
- Deterministic result: `03_results/RESULTS_V1.json`
- Independent replay: `04_review/INDEPENDENT_REPLAY_V5.json`
- Novelty audit: `04_review/NOVELTY_AUDIT.md`
- Grok review: `04_review/GROK_REVIEW.md`

## Next decisive test

Freeze one survey's published completeness function or a prospective archive cutoff. Predict first-digit counts for later or held-out planets without fitting those rows. Kill the selection account if the model misses the held-out shape beyond the frozen predictive margin. Kill the intrinsic departure claim if completeness correction removes or reverses the residual.

## Bottom line 🏆

The saved archive has strong raw first-digit departures in its three large branches. None survives the complete frozen selection-control rule. The bounded result is an informative null, and the broad finding is a rediscovery.
