# Good And Bad Examples

## Main-Line Gap

Bad:

> Existing acoustic scattering experiments, standard object comparisons, and acoustic benchmarks have already handled related problems from different perspectives.

Problem: broad, vague, and gives the reader no concrete relation.

Better:

> Existing target-scattering experiments record scattering data under limited source-receiver geometries or test planes. Standard-object studies compare analytical, approximate, and numerical solutions for spheres, cylinders, or ellipsoids under specified boundary conditions. Room-acoustic benchmarks publish room geometry, measurement configuration, hardware information, and response data for sound-field simulation.

Why better: each sentence names the prior-work type, object, and relevant output.

## Contract-Aware Related Work

Bad:

> This work provides a useful foundation for our dataset and demonstrates the importance of directional acoustic modeling.

Problem: generic and self-centered.

Better:

> The experiment measured cylinder scattering spectra under controlled source and receiver geometries. The angle organization remained tied to the selected test geometries rather than to a reusable object-level direction-pair index.

Why better: the sentence tells readers what the cited work measured and what coverage remains.

## Preserving User Meaning

Bad:

> The method may not be ideal for this task.

Problem: weakens a strong user claim.

Better:

> The method solves a different physical problem, so it is not used as a primary evaluation target for this task.

Why better: keeps the boundary but gives the technical reason.

