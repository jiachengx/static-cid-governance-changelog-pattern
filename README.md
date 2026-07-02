# Static CID Governance Changelog Pattern

**Author / Maintainer:** Stephen Chia-Cheng Hsu  
**Chinese Name:** 許家誠  
**Contact:** chiacheng.hsu@owasp.org  
**GitHub:** https://github.com/jiachengx  
**Public reference version:** v1.0.4  
**DOI:** https://doi.org/10.5281/zenodo.21140326  

## GitHub repository

Recommended public repository URL:

```text
https://github.com/jiachengx/static-cid-governance-changelog-pattern
```

## How to cite

If you use or reference this pattern, please cite:

> Hsu, Stephen Chia-Cheng. *Static CID Governance Changelog Pattern: A Public Governance Trail Method*. Version v1.0.2. 2026. GitHub: https://github.com/jiachengx/static-cid-governance-changelog-pattern

A `CITATION.cff` file is included for citation metadata.

## Overview

Static CID Governance Changelog Pattern is a public documentation pattern for turning a conventional `CHANGELOG.md` into a governance artifact.

In ordinary software projects, a changelog usually records what changed between releases. In governance-oriented publishing systems, a changelog can do more. It can become a public governance trail that records why a change was made, what governance boundary it affects, whether it changes reference behavior, whether it changes content identity handling, and whether maintainers must perform migration.

This repository provides a reusable changelog structure for nonprofit, educational, digital archive, public-interest, documentation, and static publishing projects.

## Relationship to Static CID Governance

This repository is a companion repository to:

```text
https://github.com/jiachengx/static-cid-governance-open-reference
```

The main Static CID Governance repository provides an open reference model and tools for CID-based reference consistency governance in static publishing and offline content governance environments.

This repository focuses only on the **changelog governance pattern**.

It does not implement CID generation, reference verification, public projection, release gates, inventory guarding, Offline Editor core logic, or private registry management.

Instead, it documents how governance-oriented projects can use changelog records to preserve release reasoning, public/private boundary changes, migration notes, and long-term maintenance handoff information.

## Why this repository exists

Hybrid governance systems are difficult to maintain when release notes only say what changed.

For nonprofit organizations, educational projects, digital archives, and public-interest websites, the harder questions are often:

- Why was this change made?
- What risk did this change reduce?
- Did this change affect public output?
- Did this change affect private governance data?
- Did this change alter content identity or CID behavior?
- Did this change affect reference consistency?
- Does this release require migration?
- What should future maintainers know before modifying this area?

A governance changelog helps answer these questions.

This repository exists because many organizations need not only software releases, but also maintainable governance memory.

## What this repository contains

This repository contains:

- `CHANGELOG.md` structure for public release notes.
- `GOVERNANCE_CHANGELOG.md` structure for governance-level changes.
- `CHANGELOG_TEMPLATE.md` for future releases.
- `RELEASE_NOTE_TEMPLATE.md` for GitHub releases.
- Documentation on changelog-as-governance-trail.
- Public/private boundary note patterns.
- Reference consistency release-note patterns.
- Nonprofit maintenance and handoff framing.
- Examples of governance-oriented release entries.
- CC BY-SA 4.0 licensing for sharing and adaptation.

## What this repository deliberately excludes

This repository does not include:

- Offline Editor source code.
- CID generation tools.
- release-gate verifier code.
- private registry data.
- production manifests.
- organization-specific release logs.
- credentials or secrets.
- account recovery workflows.
- project-specific internal security notes.
- formal incident details from any real organization.

This repository is a documentation pattern, not a production incident log.

## Licensing

Unless otherwise stated, this repository is licensed under:

```text
Creative Commons Attribution-ShareAlike 4.0 International
SPDX-License-Identifier: CC-BY-SA-4.0
```

This means you may share and adapt the material, including for nonprofit, educational, public-interest, and documentation use, provided that you give appropriate attribution and distribute adaptations under compatible share-alike terms.

The full license text is provided under:

```text
LICENSES/CC-BY-SA-4.0.txt
```

## Suggested attribution

When adapting this pattern, please attribute:

```text
Static CID Governance Changelog Pattern
Author: Stephen Chia-Cheng Hsu
GitHub: https://github.com/jiachengx/static-cid-governance-changelog-pattern
```

Recommended citation:

```text
Hsu, Stephen Chia-Cheng. Static CID Governance Changelog Pattern: A Public Governance Trail Method. Version v1.0.2. 2026. GitHub: https://github.com/jiachengx/static-cid-governance-changelog-pattern
```

## Core idea

A normal changelog records:

```text
what changed
```

A governance changelog records:

```text
what changed
why it changed
what risk it reduced
what boundary it affected
whether identity behavior changed
whether reference behavior changed
whether public output changed
whether migration is required
what future maintainers should know
```

## Governance changelog areas

A governance changelog should track changes in these areas.

### 1. Identity model

Tracks changes to:

- stable logical identity;
- route identity;
- CID or hash snapshot behavior;
- version metadata;
- canonicalization assumptions;
- source-reference metadata.

### 2. Reference consistency

Tracks changes to:

- latest-tracking references;
- pinned snapshot references;
- stale reference detection;
- source-reference preservation;
- public display of reference metadata.

### 3. Public/private boundary

Tracks changes to:

- what appears in public output;
- what remains private;
- whether public JSON includes or excludes certain metadata;
- whether private registry fields are protected;
- whether organization-specific or sensitive data is excluded.

### 4. Release-gate verification

Tracks changes to:

- validation rules;
- package inventory checks;
- missing-file detection;
- schema validation;
- public asset checks;
- reference verification;
- release readiness criteria.

### 5. Migration and handoff

Tracks changes that require:

- data migration;
- projection regeneration;
- schema update;
- documentation update;
- maintainer action;
- handoff notes for future nonprofit maintainers.

## Recommended release entry structure

Each release should include these sections when applicable:

```markdown
## [Version] - YYYY-MM-DD

### Summary

Briefly describe the release.

### Added

New features, files, templates, checks, or documentation.

### Changed

Behavior changes, structure changes, naming changes, or workflow changes.

### Fixed

Corrections to documentation, examples, release logic, or governance assumptions.

### Governance reason

Explain why the change was made and what governance risk it reduces.

### Identity impact

Explain whether stable identity, route identity, CID/hash snapshots, version metadata, or canonicalization assumptions changed.

### Reference impact

Explain whether latest-tracking references, pinned snapshot references, source references, or stale reference detection changed.

### Public/private boundary impact

Explain whether public output, private registry scope, sensitive fields, or excluded content assumptions changed.

### Release-gate impact

Explain whether validation rules, package checks, asset checks, or release readiness criteria changed.

### Migration notes

Explain whether users must migrate data, regenerate projections, update schemas, or rerun verification tools.

### Handoff notes

Explain what future maintainers should know before changing related files or rules.
```

## Example governance entry

```markdown
## [1.0.2] - 2026-07-02

### Summary

Updated public citation metadata and author-name formatting.

### Governance reason

The change was made to improve citation compatibility for GitHub, Zenodo, citation parsers, and academic reuse.

### Identity impact

No change to the governance changelog model.

### Reference impact

No change to reference behavior.

### Public/private boundary impact

No boundary change.

### Release-gate impact

No release-gate logic is implemented in this repository.

### Migration notes

Users may update citations from Stephen Hsu (許家誠) to Stephen Chia-Cheng Hsu.

### Handoff notes

Future releases should keep citation metadata romanized and place the Chinese name in README or NOTICE rather than in `CITATION.cff` author fields.
```

## Changelog as governance trail

This project treats changelog records as governance artifacts.

A governance changelog is useful when a project combines:

- static publishing;
- content governance;
- CID or hash snapshots;
- reference consistency;
- public/private data boundaries;
- release validation;
- package integrity;
- nonprofit maintenance handoff.

In these contexts, a changelog is not just a list of bug fixes. It becomes a record of why a system evolved and what governance assumptions future maintainers must preserve.

## Public/private boundary principle

Every governance changelog should follow this rule:

```text
Public changelog entries may describe governance changes, release reasoning, public output behavior, migration requirements, and validation scope.

Public changelog entries must not expose credentials, secrets, private registry records, organization-specific restricted content, internal account recovery workflows, sensitive incident details, or private operational logs.
```

## Relationship to FHIR

This repository is not an implementation of HL7 FHIR.

It may be used together with governance models that are informed by selected FHIR concepts such as logical identity, versioned reference, narrative readability, controlled coding, and provenance-style auditability.

However, this repository is not:

```text
a FHIR implementation
a FHIR Implementation Guide
a FHIR profile
a FHIR derivative standard
FHIR Lite
a non-medical edition of FHIR
```

FHIR is mentioned only for conceptual comparison and attribution when relevant.

## Suggested repository topics

Suggested GitHub topics:

```text
changelog
governance
release-notes
nonprofit
documentation
public-interest-tech
digital-archives
maintenance
handoff
open-source
static-publishing
```

## Suggested repository description

```text
A governance-focused changelog pattern for nonprofit static publishing, maintenance handoff, and release accountability.
```

## How to use this repository

Use this repository when you want to create:

- a public governance changelog;
- a release note policy;
- a nonprofit maintenance handoff format;
- a public/private boundary release record;
- a static publishing governance history;
- a documentation pattern for audit-friendly project evolution.

Recommended workflow:

```text
1. Copy CHANGELOG_TEMPLATE.md into your project.
2. Copy or adapt GOVERNANCE_CHANGELOG.md.
3. Remove any organization-specific or sensitive details.
4. Use the release entry structure for each public release.
5. Link your release notes to public repository tags or archived releases.
6. Preserve attribution according to CC BY-SA 4.0.
```

## Scope and non-goals

This repository is intended to provide a reusable changelog governance pattern.

It is not intended to be:

- a software package;
- a release automation tool;
- a security incident disclosure repository;
- a private project log;
- a replacement for legal agreements;
- a replacement for formal compliance audits;
- a place to publish credentials, secrets, internal registry data, or organization-specific operational details.

## Citation metadata

This repository includes:

```text
CITATION.cff
```

Recommended citation:

```text
Hsu, Stephen Chia-Cheng. Static CID Governance Changelog Pattern: A Public Governance Trail Method. Version v1.0.2. 2026. GitHub. https://github.com/jiachengx/static-cid-governance-changelog-pattern
```

## Release

Current public reference release:

```text
v1.0.2
```

GitHub releases:

```text
https://github.com/jiachengx/static-cid-governance-changelog-pattern/releases
```

Latest release:

```text
https://github.com/jiachengx/static-cid-governance-changelog-pattern/releases/latest
```

## Trademark and attribution notice

HL7®, FHIR®, and related marks are trademarks of Health Level Seven International. This repository is independent and is not endorsed, certified, sponsored, or approved by HL7.

Any reference to FHIR is made only for conceptual comparison and attribution.

## Author

```text
Stephen Chia-Cheng Hsu
Chinese name: 許家誠
Contact: chiacheng.hsu@owasp.org
GitHub: https://github.com/jiachengx
```

## Copyright

Copyright © 2026 Stephen Chia-Cheng Hsu.

Unless otherwise stated, this repository is licensed under CC BY-SA 4.0. See `LICENSE.md`, `NOTICE`, and `COPYRIGHT` for details.
