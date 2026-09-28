# Legal notice

This file summarizes practical release considerations for the beta. It is not legal advice. Obtain advice from qualified counsel before a commercial launch or if trademark, licensing, export, consumer-protection, or warranty questions apply to your distribution.

## Project license and warranty

Copyright © 2026 CJ Storie. All rights reserved. SpaceMouse Studio is distributed under the included [Proprietary Beta License](LICENSE), not an open-source license. The license permits installation and use for the recipient's own Roblox Studio development but prohibits redistribution, resale, rebranding, modification, and false claims of authorship. Its warranty disclaimer and limitation of liability apply only to the extent permitted by applicable law.

The public beta package intentionally omits the Windows bridge source code, build scripts, and internal protocol documentation. Roblox requires publicly shared plugin code to remain readable; readability does not grant permission to redistribute or relicense it.

## Independent compatibility project

SpaceMouse Studio is independently developed. It is not affiliated with, authorized by, certified by, sponsored by, or endorsed by 3Dconnexion, Microsoft, or Roblox Corporation.

3Dconnexion and SpaceMouse are trademarks of their respective owner. Roblox is a trademark of Roblox Corporation. References to those names describe compatibility, required third-party software, or the host application only. The product icon is original and intentionally contains no third-party logo or Roblox branding.

Do not add a 3Dconnexion or Roblox logo, certification badge, official-partner claim, or other endorsement language without written permission. Roblox's published brand guidance generally prohibits use of its logo outside approved programs, and Roblox's Creator Store terms require uploaders to have the necessary rights to everything they submit.

## 3Dconnexion software and certification

The 3DxWare driver is required but is **not included**. Users obtain it directly from 3Dconnexion and accept its license separately.

This beta contains no 3Dconnexion SDK source, header, library, firmware, or driver binary. It reads a Windows HID Multi-axis Controller through Microsoft Raw Input. It must not be described as “3Dconnexion Certified.” 3Dconnexion's published certification requirements call for its Navigation Library or 3DconnexionJS based on SDK v4.0 or higher, plus navigation, command, documentation, and credit requirements. Contact 3Dconnexion's partner team before seeking certification or changing to its SDK.

References:

- [3Dconnexion Software Developer Program](https://3dconnexion.com/us/software-developer-program/)
- [3Dconnexion certification requirements](https://3dconnexion.com/uk/wp-content/uploads/sites/1/2020/08/3Dconnexion-Certification-Requirements.pdf)

## Roblox distribution

Only the Luau plugin belongs in the Roblox Creator Store. The Windows bridge must be distributed separately. The listing and onboarding must disclose the Windows bridge requirement before installation or purchase.

Keep the plugin source readable and self-contained. Do not add obfuscation, remote `require(assetId)`, `loadstring()`, `InsertService:LoadAsset()`, or other prohibited remote-loading patterns.

References:

- [Roblox Studio plugin publishing](https://create.roblox.com/docs/studio/plugins)
- [Roblox Creator Store requirements](https://create.roblox.com/docs/production/creator-store)
- [Roblox Creator Store Terms](https://en.help.roblox.com/hc/en-us/articles/21308223046932-Creator-Store-Terms)
- [Roblox name and logo guidelines](https://en.help.roblox.com/hc/en-us/articles/115001708126-Roblox-Name-and-Logo-Community-Usage-Guidelines)

## Microsoft .NET runtime

The self-contained Windows bridge includes Microsoft .NET runtime components under their respective licenses. The corresponding Microsoft license and third-party notices are included beside the bridge executable and must remain with redistributed binary packages.

## Redistribution checklist

Before sharing a beta build:

1. Keep `LICENSE`, `LEGAL.md`, `PRIVACY.md`, and `THIRD_PARTY_NOTICES.md` in the package.
2. Keep the Microsoft .NET license and third-party notices in `bridge\beta-dist`.
3. Clearly label the build **Beta**, **Windows only**, and **unsigned**.
4. Disclose that 3DxWare and a compatible device are separately required.
5. Do not claim official status or certification.
6. Publish checksums from the same final archive users download.
7. Do not distribute the private source tree or copyright-registration working papers.
