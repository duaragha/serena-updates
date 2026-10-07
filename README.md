# Serena updates

Public installers and update manifests for Serena desktop. Application source and build workflows are maintained separately in a private repository.

- [All releases](https://github.com/duaragha/serena-updates/releases)
- [Latest stable release](https://github.com/duaragha/serena-updates/releases/latest)

Linux and Windows use this repository without a GitHub login. Stable releases and Serena Dev prereleases use separate update channels.

## Feed migration

The initial mirrored releases, stable `v0.3.21` and Dev `v0.3.10-dev.45`, preserve the original installer bytes. They still contain the previous feed address and do **not** fix an installed app's update checks. A migration-capable build will be published after release publishing is configured.

Existing installations will need that installer once to switch feeds. Afterward, the app's normal update checks use this repository. No running app is replaced or restarted automatically.

This repository holds release documentation, installers, and updater metadata only. GitHub's generated source archives contain the documentation, not the application source.
