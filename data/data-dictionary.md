# Data Dictionary

## training_sets.csv
This is the primary combined training + readiness log.

One row equals one working set. Session-level readiness fields are repeated across all working-set rows from the same session so training and readiness can be viewed together. Analysis must de-duplicate session-level variables by `date + session_day` before calculating readiness averages.

### Session / readiness fields
- `date`: training date, ISO format YYYY-MM-DD
- `session_day`: day number inside current training week
- `morning_bodyweight_lb`: morning bodyweight, ideally after bathroom and before food/fluid
- `sleep_hours`: total sleep from the previous night
- `sleep_quality_1_5`: subjective sleep quality
- `morning_energy_1_5`: energy shortly after waking
- `morning_soreness_1_5`: general training soreness
- `groin_morning_0_10`: groin symptoms on waking
- `knee_morning_0_10`: knee symptoms on waking
- `back_morning_0_10`: back symptoms on waking
- `training_time`: approximate start time of training
- `hydration_pretraining_1_5`: subjective hydration immediately before training
- `fluids_pretraining_oz`: total fluid consumed before training when known
- `caffeine_mg`: total caffeine consumed before training
- `caffeine_time`: time of the most recent pre-training caffeine dose
- `pretraining_energy_1_5`: energy immediately before training
- `pretraining_stress_1_5`: stress immediately before training

### Set-level fields
- `exercise`: readable exercise name
- `category`: competition, variation, or accessory
- `variation`: exact movement variation
- `load_lb`: external load in pounds
- `reps`: reps completed
- `set_number`: working-set sequence
- `rpe`: set-specific RPE; required for competition lifts
- `last_set_rpe`: accessory/non-comp default RPE field, generally populated only on final set
- `pain_0_10`: movement-specific pain when relevant
- `notes`: technique, equipment, per-hand load, or other context

Do not backfill guessed values.

## daily_readiness.csv
Deprecated for primary logging as of October 2026. Readiness is now captured directly in `training_sets.csv` so the full session context can be viewed in one place. The file is retained only to avoid deleting repository history.

## bodyweight.csv
Optional derived trend file. Morning bodyweight should be entered in the combined training log first; rolling averages can be generated later for analysis.
