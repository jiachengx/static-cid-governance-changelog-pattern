# Example Governance Release Entry: v1.0.0

## Summary

Initial public release of a static publishing governance model.

## Governance reason

The release establishes stable logical identity, content-derived snapshots, public-safe projection, and release-gate validation as a reusable governance loop.

## Identity impact

- Stable identity introduced.
- CID/hash snapshot behavior introduced.
- Version metadata introduced.

## Reference impact

- Latest-tracking reference policy introduced.
- Pinned snapshot reference policy introduced.
- Source-reference metadata introduced.

## Public/private boundary impact

- Public output may expose public-safe identity and reference metadata.
- Private registries and internal governance logs remain excluded.

## Release-gate impact

- Initial validation checks introduced.

## Migration notes

No migration required for first release.

## Handoff notes

Future maintainers should preserve the separation between public projection and private governance records.
