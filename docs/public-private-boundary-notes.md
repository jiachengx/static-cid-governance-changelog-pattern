# Public/Private Boundary Notes

A governance changelog should explicitly state whether a release changes public/private boundaries.

Public outputs may expose stable identity, route, CID or hash snapshots, and public reference metadata. They should not expose private registries, internal governance logs, credentials, secrets, account recovery workflows, or organization-specific restricted content.

Each release should state:

- whether public output fields changed;
- whether any private field was removed from public output;
- whether public-safe projection rules were strengthened;
- whether maintainers must regenerate public JSON or static pages.
