# Governance Changelog

This file records governance-level changes, not only software changes.

A governance changelog should document changes that affect content identity, reference behavior, public/private boundaries, release verification, migration requirements, and long-term maintainability.

## Entry format

Each release entry should include the following sections.

### Summary

What changed in this release.

### Governance reason

Why the change was made and what governance risk it reduces.

### Identity impact

Whether this release changes stable identity, route identity, CID/hash snapshots, version metadata, or canonicalization assumptions.

### Reference impact

Whether this release changes latest-tracking references, pinned snapshot references, source-reference metadata, or stale-reference detection.

### Public/private boundary impact

Whether this release changes what is exposed in public output and what remains private.

### Release-gate impact

Whether this release adds, removes, or changes validation checks.

### Migration notes

Whether existing users need to migrate data, regenerate projections, update schemas, or rerun verification tools.

### Handoff notes

What future nonprofit maintainers should know before modifying related files or rules.

## Governance principle

> A changelog should explain not only what changed, but also why the change matters for governance, integrity, public output, and future maintainability.
