# Security model

## Guarantees in v0.1

- The bridge binds its TCP listener to `127.0.0.1` only.
- It exposes read-only device state and accepts only `GET`.
- It has no outbound network code, update checker, analytics, filesystem API, or command-execution route.
- It emits no CORS permission, which prevents ordinary browser JavaScript from reading the response cross-origin.
- The plugin uses a fixed numeric-loopback URL; users cannot redirect it to a remote host through settings.
- Both sides validate and bound untrusted lengths and numeric input.
- Stale input decays to zero in both bridge and plugin.

## Residual risk

Any process running as the same Windows user can query a loopback service. Axis/button state is low-sensitivity, and v0.1 has no mutating commands, so the prototype does not add authentication. If a later bridge accepts configuration, launch, update, or filesystem commands, it must add a per-install secret and request authentication before any such endpoint ships.

The v0.1 build is unsigned. Windows may warn before it starts. Do not bypass warnings for binaries obtained from an untrusted distributor; build from source until signed releases exist.

## Reporting

For a public release, add a monitored private vulnerability-reporting address and a supported-version policy here before publication.
