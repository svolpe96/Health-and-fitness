# Health and Fitness — Powerlifting Coaching System

This repository is the source of truth for Steven's long-term powerlifting training, recovery, physique development, and coaching decisions.

## Primary objective
Develop toward elite 75 kg powerlifting performance, with Team USA as the long-term target.

## Current phase
Return-to-strength / reaccumulation, starting October 5, 2026.

## Repository map
- `athlete/` — profile, goals, injury history, technique
- `program/` — current and archived programming
- `data/` — raw training and readiness data
- `coaching/` — decisions, hypotheses, and adjustments
- `reviews/` — weekly and block reviews
- `analysis/` — future scripts, reports, and dashboards
- `reference/` — historical programming and source material

## Logging rules
1. One row per working set in `data/training_sets.csv`.
2. Competition squat, bench, and deadlift: record RPE for every working set.
3. Accessory and non-competition work: record last-set RPE by default.
4. Never invent missing RPE, pain, velocity, sleep, or bodyweight data.
5. Historical maxes are context only and are not treated as current 1RMs.
6. Major program changes require a documented reason in `coaching/decisions.md`.
7. Exact exercise variation/setup must be stated when relevant: grip, stance, attachment, implement, angle, tempo, and bilateral vs unilateral. Avoid generic labels like "lat pulldown" when a specific variation is intended.
8. Coach selects the exact variation judged best for the current goal and context. Do not present multiple variation choices by default. Only substitute when equipment, pain, safety, or a clearly better coaching reason requires it.

## Current performance context
Historical gym bests: 585 squat / 355 bench / 610 deadlift.
Best competition lifts at 75 kg: 529 squat / 325 bench / 606 deadlift.

These numbers are not current training maxes.
