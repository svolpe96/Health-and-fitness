# Data Dictionary

## training_sets.csv
One row equals one working set.

- `date`: training date, ISO format YYYY-MM-DD
- `session_day`: day number inside current training week
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

Do not backfill guessed RPE values.

## daily_readiness.csv
Raw recovery variables are kept separately instead of collapsing them into a single readiness score.

Future fields may include velocity data, nutrition, hydration, and wearable-derived metrics.
