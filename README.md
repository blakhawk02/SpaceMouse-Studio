# SpaceMouse Studio

Official download channel for the **SpaceMouse Studio** Windows companion bridge.

SpaceMouse Studio adds proportional six-axis SpaceMouse camera navigation to Roblox Studio. The Roblox Studio plugin is installed separately through Roblox Studio. This repository intentionally contains public documentation and compiled beta releases only; the proprietary source code is not published here.

## Download the Windows companion

Download the newest beta from the [official releases page](https://github.com/blakhawk02/SpaceMouse-Studio/releases).

The expected release file is:

```text
SpaceMouse-Studio-Bridge-Windows-x64.zip
```

Only download the bridge from this repository. Check the SHA-256 value shown in the release notes before running it.

## Install

1. Install the current 3DxWare driver from 3Dconnexion and confirm the controller works in the 3Dconnexion trainer.
2. Download `SpaceMouse-Studio-Bridge-Windows-x64.zip` from the latest release.
3. Extract the entire ZIP to a folder. Do not run the application from inside the ZIP.
4. Open `bridge\SpaceMouseStudioBridge.exe`.
5. Leave the bridge running while using Roblox Studio.
6. Open the separately installed SpaceMouse Studio plugin and enable camera control.

Start the bridge once after signing into or restarting Windows. You do not need to restart it for every Roblox Studio session.

## Windows beta warning

The current beta is not code-signed. Windows may display an **Unknown Publisher** or Microsoft Defender SmartScreen warning. Verify that the download came from this repository and that its SHA-256 checksum matches the release notes.

## Security and privacy

- The bridge listens only on `127.0.0.1:37567`.
- It does not accept connections from other computers.
- It makes no outbound internet connections.
- It collects no telemetry, account information, or Roblox project content.

See [PRIVACY.md](PRIVACY.md) and [SECURITY.md](SECURITY.md).

## License and ownership

Copyright © 2026 CJ Storie. All rights reserved.

Installing or using the beta means accepting the [SpaceMouse Studio Proprietary Beta License](LICENSE). Redistribution, resale, modification, rebranding, and removal of ownership notices are prohibited.

SpaceMouse Studio is an independent compatibility project. It is not made, sponsored, certified, or endorsed by 3Dconnexion or Roblox. 3Dconnexion and SpaceMouse are trademarks of their respective owner. Roblox is a trademark of Roblox Corporation.

See [LEGAL.md](LEGAL.md) and [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md) for additional notices.
