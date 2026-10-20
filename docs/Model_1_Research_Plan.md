
# Model 1 — Pitching Relationships

## Primary Research Question

How do changes in a pitcher's mechanics and release characteristics relate to changes in velocity, spin, and pitch movement?

## Objective

Develop a predictive model that learns how pitching characteristics change together within individual pitchers over time.

The model should account for differences between pitchers, pitch types, and existing mechanical profiles.

## Unit of Analysis

Pitcher × Pitch Type × Time Window

Rather than treating every pitch as an independent observation, we will aggregate pitches into time windows for individual pitchers and pitch types.

Initial proposal: consecutive five-start windows.

Window size will be evaluated during exploratory analysis.

## Initial Variables

### Pitcher Identification
- Pitcher ID
- Pitcher handedness
- Game date
- Pitch type

### Release Characteristics
- Arm angle
- Release extension
- Release position X
- Release position Z

### Pitch Characteristics
- Release speed
- Spin rate
- Spin axis
- Horizontal movement
- Vertical movement

### Additional Context
- Pitch count per window
- Pitch usage percentage
- Batter handedness
- Game conditions where available

## Initial Prediction Targets

Predict changes between consecutive windows in:

- Release velocity
- Spin rate
- Horizontal movement
- Vertical movement

These outcomes should be modeled jointly where feasible.

## Modeling Principles

1. Pitching characteristics are interconnected.
2. Different pitchers may respond differently to similar changes.
3. Predictions must account for pitch type and baseline characteristics.
4. Avoid treating correlated variables as independently adjustable.
5. Evaluate out-of-sample prediction accuracy.
6. Observational relationships do not establish causal effects.

## Initial Validation Strategy

- Split training and testing periods chronologically.
- Prevent overlapping time windows from leaking information.
- Compare predictions against a no-change baseline.
- Evaluate individual and joint prediction accuracy.
- Investigate prediction uncertainty.
- Examine performance separately by pitch type.

## Success Criteria

Model 1 should demonstrate useful predictive accuracy on unseen data and produce plausible combinations of pitch-characteristic changes.

If it cannot outperform simple baselines, reconsider the modeling approach before proceeding.
