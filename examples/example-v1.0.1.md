# Example Governance Release Entry: v1.0.1

## Summary

Strengthened stale-reference detection and improved release notes for public projection changes.

## Governance reason

The change reduces the risk that static public pages continue to reference outdated or missing content snapshots.

## Identity impact

No change to stable identity or hash calculation.

## Reference impact

- Stale-reference detection strengthened.
- Public projection should be regenerated after reference updates.

## Public/private boundary impact

No private fields were added to public output.

## Release-gate impact

Release gate now fails when a public projection references a snapshot not present in the current source index.

## Migration notes

Regenerate public projection and rerun reference verification.

## Handoff notes

Do not bypass stale-reference checks to force a release. Regenerate projections instead.
