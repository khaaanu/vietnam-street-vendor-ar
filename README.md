# Street vendors of Ho Chi Minh City: site-specific AR prototypes

Self-hosted builds of three augmented reality prototypes from Quynh Nhu Bui's doctoral research at RMIT University, first published on 8th Wall and moved here before 8th Wall's hosting service ends on 28 February 2027.

| Prototype | Path | Former 8th Wall address |
|---|---|---|
| Portal to Saigon | `portal-saigon/` | https://nhubui.8thwall.app/portal-vietnam/ |
| The Vendor Cart as Sensory Assemblage, Footscray | `audio-vendor/` | https://nhubui.8thwall.app/audio-vendor/ |
| Nostalgia in Little Saigon, Richmond | `sky-vendor/` | https://nhubui.8thwall.app/sky-vendor/ |

Project website: https://vietnam3dheritage.myportfolio.com/

## How these builds were made

Each folder is the `dist/` output of `npm run build` on the project's 8th Wall buildable code export. Two build settings were changed so the sites run from a subfolder and build without the 8th Wall cloud editor:

- `output.publicPath` set to `'./'` (relative paths) in `config/webpack.config.js`
- `ts-loader` set to `transpileOnly: true`, so TypeScript is compiled without type checking, as in the 8th Wall editor

No project code or assets were changed.

## Licences and credits

- 3D reconstructions, sound and design: Quynh Nhu Bui, licensed under Creative Commons Attribution-NonCommercial 4.0 (https://creativecommons.org/licenses/by-nc/4.0/).
- 8th Wall XR Engine: created by Niantic Spatial, Inc., copyright Niantic Spatial, Inc. Distributed unmodified under the 8th Wall XR Engine License Agreement (`XR-ENGINE-LICENSE.txt`), which provides the software "as is" without warranty. This project is not connected with, sponsored or endorsed by Niantic Spatial.
- 8th Wall runtime: copyright 2025 Niantic Spatial, Inc., MIT licence (`RUNTIME-LICENSE.txt`).
