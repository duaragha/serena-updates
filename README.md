# Serena updates

Public installers and update manifests for Serena desktop. Application source and build workflows are maintained separately in a private repository.

- [Serena Dev v0.3.10-dev.48 — Linux and Windows](https://github.com/duaragha/serena-updates/releases/tag/v0.3.10-dev.48)
- [All releases](https://github.com/duaragha/serena-updates/releases)
- [Latest stable release](https://github.com/duaragha/serena-updates/releases/latest)

Linux and Windows download from this repository without a GitHub login. Stable and Serena Dev have separate app identities, profiles, and update channels.

## Feed migration

Dev `v0.3.10-dev.48` includes the public update feed. Both platform builds passed, both installer SHA-512 checksums were verified against their public updater manifests, and both packaged apps were inspected for the public feed address.

Stable delivery uses Serena Dev's **Releases > Promote to Main**. The selectable fix is **Fix updates with the public installer repository**. Existing installations that still target the old private repository need a migration-capable installer once to switch feeds. Subsequent update checks use this public repository.

The initial mirrored builds, stable `v0.3.21` and Dev `v0.3.10-dev.45`, preserve the original installer bytes and still use the old feed. Dev `.46` and `.47` are incomplete Linux-only builds; `.48` is the complete migration build for both platforms.

This repository holds release documentation, installers, and updater metadata only. GitHub's generated source archives contain the documentation, not the application source.
