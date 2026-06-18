
SRS-drive OpenSpec schema
=========================

This [OpenSpec](https://github.com/Fission-AI/OpenSpec) schema is an extension of the default `spec-driven` schema
with a few changes:

* The `proposal.md` (what and why) format is expanded and more detailed-oriented
* The `design.md` file (how) can either be an ADR-style format (for delta-specs) or a single-coherent format (for new concepts)
* The `tasks.md` file records what changed and why upon marking a task as complete, creating an audit trail
* The `spec.md` file uses an EARS format for writing specs instead of Given-When-Then; Specs are "tagged" for traceability in code and tests.

The format changes are expanded over the defaults, covering more edge cases and design space, to drive agents towards a more specified, stable outcome.
The expanded scope of the documents focuses more on core invariants, validation/verification, and tracks when gaps in the spec caused implementation drift.

The core content of the format follows typical [CONOPS](https://en.wikipedia.org/wiki/Concept_of_operations) documents,
aligns closely to the **IEEE/ISO/IEC 29148-2018** Requirements Specification, and SWEBOK 4.0 Requirements recommendations.

### Example

The [devbox](https://github.com/ohpauleez/devbox) project uses the `srs-driven` schema and serves as a good example of what to expect.

### Installation

Copy the `srs-driven` directory into the `openspec/schemas` directory within your project.
See [OpenSpec Customization](https://github.com/Fission-AI/OpenSpec/blob/main/docs/customization.md) docs for more details.

Then update your project's `openspec/config.yaml` with:
```
schema: srs-driven
```

### Further suggestions

* Create a living-doc called `docs/design.md` that captures the current state _total_ design of the system. Include updates to this doc along with your code and tests
* Create a top-level [codemap](https://matklad.github.io/2021/02/06/ARCHITECTURE.md.html) called `ARCHITECTURE.md`, to anchor the overall structure of the project for humans and agents. See this [example](https://github.com/ohpauleez/devbox/blob/main/ARCHITECTURE.md)

