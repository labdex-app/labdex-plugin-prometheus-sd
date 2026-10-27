# Prometheus service discovery

A [labdex](https://github.com/reykimedev/labdex) plugin. HTTP service-discovery endpoints for Prometheus / VictoriaMetrics, so monitoring follows the inventory.

**Version** 1.0 · **Works with** labdex >=1.3,<2 · **Plugin id** `prometheus-sd`

> [!WARNING]
> Built with AI, for home labs only: labdex and its plugins were written largely with an AI
> coding assistant (Claude), directed and reviewed by a human. They haven't had an independent
> security audit and may contain security problems. Run them on a trusted home network.

## Install

It ships with labdex: **Plugins › Marketplace**, then *Install* (nothing is downloaded). Updates arrive through the official Marketplace (signed with the labdex project key).

## Settings

| Setting | Notes |
| --- | --- |
| Node exporter port |  |
| Host statuses to include |  |
| Only these zones | Empty = all zones |
| Use DNS names instead of IP addresses |  |

## Actions

—

## Releasing

Bump `version` in `plugin.yaml`, add a `## <version>` section to `CHANGELOG.md`, commit, then
`git tag v<version> && git push --tags`. The release workflow signs the plugin with the
`LABDEX_SIGNING_KEY` secret and attaches `prometheus-sd-<version>.zip` to a GitHub release.
