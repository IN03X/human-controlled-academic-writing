# Artifact Consistency Gate

## Trigger

Load when manuscript claims refer to data, code, figures, tables, generated outputs, file paths, experiments, benchmarks, or implemented capabilities.

## Required Checks

- The referenced artifact exists at the stated location.
- The data or script produces the stated result.
- Figure and table labels, units, captions, legends, and manuscript references agree.
- Figures remain readable at paper scale; labels, arrows, and input-output relations are clear.
- Numerical values and comparison directions match the artifact.
- Numerical precision is consistent across prose, figures, and tables.
- Completed, placeholder, partial, and planned work are labeled accurately.
- A claimed capability exists in the current implementation rather than only in an interface or design.
- Internal file paths, experiment names, and run labels do not leak into manuscript prose, tables, captions, or references.

## Decision Rule

Never upgrade project intent into implementation fact. If only an interface exists, say an interface is provided. If a result is preliminary or absent, weaken the manuscript claim or mark the gap for the user.

## Stop Conditions

Stop before writing a definitive claim when the artifact is missing, stale, inconsistent, or unable to reproduce the stated output.
