# Astronomical Context Model

## Purpose

This model defines what astronomy contributes to YASMP without importing astrological causality into an astronomical dataset.

JPL Horizons can calculate ephemerides using specified targets, observer locations, times, time scales, coordinate systems and output types. The system is therefore suitable as a reproducible source for the physical context layer.

Source:

https://ssd.jpl.nasa.gov/horizons/manual.html

API:

https://ssd-api.jpl.nasa.gov/doc/horizons.html

## Three levels

### Level 1 — Physical astronomy

Examples:

- celestial coordinates;
- angular separation;
- altitude and azimuth;
- lunar phase;
- rise and set;
- orbital state;
- observer-relative geometry.

Status: DERIVED from an astronomical model.

### Level 2 — Environmental mediation

Possible variables:

- daylight;
- twilight;
- seasonal timing;
- lunar illumination;
- environmental variables correlated with astronomical cycles.

Status: requires independent measurement and modelling.

### Level 3 — Symbolic interpretation

Examples:

- zodiac meanings;
- planetary archetypes;
- numerological associations with dates.

Status: CLAIMED unless independently validated.

These three levels must never be silently merged.

## Astronomy as a control layer

The strongest use of astronomy in YASMP may initially be methodological rather than predictive.

It can help distinguish:

- calendar effects;
- seasonal effects;
- daylight effects;
- lunar-cycle hypotheses;
- arbitrary symbolic interpretations.

If an alleged psychological effect disappears when ordinary environmental variables are controlled, the astronomical-symbolic interpretation loses explanatory value.

## Observer dependence

Astronomical coordinates are not absolute labels detached from the measurement system.

The selected observer, reference frame, time scale and coordinate representation matter.

YASMP therefore stores the calculation settings with the result.

## Privacy

An exact birth location or observation location can be sensitive.

Implementations should prefer:

- coarse geographic cells;
- temporary calculations;
- deletion of raw coordinates after derivation;
- explicit consent for storage.

## Epistemic rule

**Astronomical measurement can establish astronomical state. It does not establish psychological meaning.**

Psychological meaning requires separate evidence.
