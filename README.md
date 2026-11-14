# Splatty

**Capture keepsakes. Keep the light.**

Splatty turns figures, badges, bricks, and other collectibles into interactive [3D Gaussian Splats](https://repo-sam.inria.fr/fungraph/3d-gaussian-splatting/) — shoot on iPhone, train on a Mac at home, browse in-app.

中文一句话：用手办级收藏品的多视角照片，在家里 Mac mini 上训出 3DGS，再在 iPhone App 里转着看。

## Status

Early MVP scaffolding. APIs and folder layout may change.

## Architecture

```text
iPhone (Splatty App)          Mac mini (Apple Silicon)         iPhone
  capture + ARKit poses  --->  msplat train  --->  .ply/.spz  --->  MetalSplatter preview
  asset library                export splat                     asset library
```

| Layer | Role | Stack (planned) |
|-------|------|-----------------|
| **App** | Guided capture, library, preview | SwiftUI · ARKit · [MetalSplatter](https://github.com/scier/MetalSplatter) |
| **Train** | Reconstruct splat offline | [msplat](https://github.com/rayanht/msplat) on Mac mini |
| **Assets** | Naming / versions / meta | see `docs/architecture.md` |

On-device **training** is intentionally out of MVP scope (viewing on device is in).

## Repo layout

```text
Apps/Splatty/     iOS app (placeholder)
Mac/train/        Mac mini training notes & scripts
docs/             architecture & capture notes
```

## Non-goals (for now)

- Selling or posting collectibles for commerce
- Buying hardware without Neil’s go-ahead
- Shipping closed-source training inside the iPhone MVP

## License

First-party material in this repository is released under the GNU General Public License, version 3 only (**GPL-3.0-only**).

Copyright (c) 2026 Near.

The license text is the unmodified GNU GPL version 3 in [`LICENSE`](LICENSE). This repository's grant is version 3 only. The sample notice in that file's appendix, which includes "or (at your option) any later version," is part of the unmodified Free Software Foundation text. The grant for Splatty is this section and [`LICENSES/README.md`](LICENSES/README.md).

Copies already received under the MIT License keep those MIT rights. The previous root `LICENSE`, including `Copyright (c) 2026 Near` and the MIT permission notice, is preserved byte for byte in [`LICENSES/MIT-legacy.txt`](LICENSES/MIT-legacy.txt). That file records the earlier grant. History was not rewritten, so earlier revisions still contain the MIT license.

中文：本仓库第一方材料以 GNU GPL 第 3 版且仅第 3 版提供（SPDX `GPL-3.0-only`）。版权行仍是 `Copyright (c) 2026 Near`。此前已按 MIT 取得的副本继续保有该 MIT 权利；原 MIT 许可证全文按字节保存在 [`LICENSES/MIT-legacy.txt`](LICENSES/MIT-legacy.txt)。范围说明见 [`LICENSES/README.md`](LICENSES/README.md)。
