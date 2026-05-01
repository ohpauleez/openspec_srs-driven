
SRS-drive OpenSpec schema
=========================

This [OpenSpec](https://github.com/Fission-AI/OpenSpec) schema is an extension of the default `spec-driven` schema
with a few changes:

* The `proposal.md` default format is expanded
* The `design.md` file can either be an ADR-style format or a single-coherent format
* The `tasks.md` file records what changed and why upon marking a task as complete, creating an audit trail
* The `spec.md` file uses an EARS format for writing specs instead of Given-When-Then; Specs are "tagged" for traceability in code and tests

### Installation

Copy the `srs-driven` directory into your `openspecs/schemas` directory.
See [OpenSpec Customization](https://github.com/Fission-AI/OpenSpec/blob/main/docs/customization.md) docs for more details.

### Further suggestions

* Create a living-doc called `docs/design.md` that captures the current state _total_ design of the system. Include updates to this doc along with your code and tests

