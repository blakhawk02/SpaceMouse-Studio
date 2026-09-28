# Privacy notice

Effective date: September 27, 2026

SpaceMouse Studio Beta does not collect, store, sell, or transmit personal information.

## Data the bridge handles

The Windows bridge reads these values from a locally connected compatible 3D controller:

- Six normalized motion axes: `X`, `Y`, `Z`, `Rx`, `Ry`, and `Rz`.
- A device path used to confirm that the input came from a supported USB vendor.
- A raw button bit mask reserved for future local mappings.

This information remains on the user's computer. It is served only through `http://127.0.0.1:37567`, an IPv4 loopback address that is not reachable from another computer on the network.

## Data the Studio plugin handles

The plugin reads the local axis values and stores only the user's navigation settings through Roblox Studio's local plugin-setting API. It does not read or transmit Roblox account credentials, project source, place content, files, contacts, or browsing activity.

## Network activity

Neither the plugin nor the bridge contains analytics, advertising, telemetry, crash reporting, an update checker, or external network requests. The only connection is from Roblox Studio to the local bridge on `127.0.0.1`.

## Future changes

Any future telemetry or online service must be opt-in, documented here before release, and disabled by default unless the user expressly chooses otherwise.

