# Changelog

All notable changes to this repository are documented here.

This repository treats changelog practice itself as a governance artifact. The entries below record changes to the public template and documentation pattern, not changes to any production system.

## [1.0.0] - 2026-07-02

### Added

- Initial public release of the Static CID Governance Changelog Pattern.
- Added `GOVERNANCE_CHANGELOG.md` as the central governance-trail format.
- Added reusable templates for release notes and governance changelog entries.
- Added documentation for changelog-as-governance-trail, public/private boundary notes, reference-consistency release notes, and nonprofit maintenance handoff.
- Added neutral examples for v1.0.0 and v1.0.1 style entries.

### Governance Notes

- This repository is intentionally independent from any production Offline Editor or private registry.
- The goal is to publish a reusable changelog method without exposing sensitive operational records.

### Public/Private Boundary Notes

- Only neutral templates and examples are included.
- Production release logs, internal account workflows, credentials, private registries, and organization-specific content are excluded.


## [1.0.2] - 2026-07-02

### Changed

- Updated public author metadata to use the citation-friendly romanized name `Stephen Chia-Cheng Hsu`.
- Updated `CITATION.cff` to remove the invalid `name-particle` field and align with GitHub / Zenodo citation tooling.
- Updated README, LICENSE, NOTICE, COPYRIGHT, and inventory metadata for consistent author attribution.

### Governance Notes

- Chinese name `許家誠` is preserved in README / NOTICE style metadata, while citation metadata uses romanized author fields for compatibility.
- This change improves public citation, academic reuse, and repository metadata stability without changing the governance changelog model.

## [1.0.1] - 2026-07-02

### Added

- Added `CITATION.cff` with the public GitHub namespace `jiachengx`.
- Added `GITHUB_UPLOAD_GUIDE.md` with repository URL, topics, upload commands, and first-release notes.
- Added `docs/WHY_THIS_PROJECT.md` for public explanation and citation context.

### Governance Notes

- This release prepares the repository for public publication under the author's GitHub account while preserving neutral naming, layered licensing, and public/private boundary separation.
