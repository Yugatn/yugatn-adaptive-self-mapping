# YASMP Data Schema v2

The schema keeps observations, derived variables and interpretations separate.

## Subject

- subject_id: pseudonymous identifier
- consent_status
- observation_period
- profile_version

No real identity is required for the analytical layer.

## Observation

- observation_id
- subject_id
- timestamp_utc
- context_id
- source
- observed_variable
- observed_value
- measurement_method
- evidence_status

## Relation

- relation_id
- source_subject_id
- target_subject_id
- relation_type
- strength
- reciprocity
- timestamp
- group_id
- criterion_version

A relation is not a personality trait.

## Symbolic Proposition

- proposition_id
- system
- proposition
- source_version
- subject_rating
- evaluator_rating
- confidence
- validation_status

## Astronomy

- observation_id
- ephemeris_provider
- ephemeris_version
- time_scale
- observer_region
- reference_frame
- target
- coordinate_type
- coordinate_value
- uncertainty
- calculation_timestamp

Privacy rule: precise location should not be stored unless necessary and explicitly consented to.

## Derived Variable

- derived_id
- input_ids
- formula_version
- value
- uncertainty
- derivation_status

## Prediction

- prediction_id
- created_at
- target_variable
- predicted_value
- confidence
- horizon
- falsification_rule
- observed_value
- outcome
- validation_status

## Evidence Ledger

Every proposition or result must have one of:

- OBSERVED
- DERIVED
- CLAIMED
- NOT_TESTED
- CONFLICTED
- Residual

Evidence status describes epistemic status, not human status.
