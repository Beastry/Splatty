# License scope

First-party material in this repository is released under the GNU General Public License, version 3 only.

| Item | Terms |
|---|---|
| SPDX identifier | `GPL-3.0-only` |
| License text | [`LICENSE`](../LICENSE) at the repository root |
| Copyright line already on the MIT grant | `Copyright (c) 2026 Near` |
| Preserved MIT grant | [`MIT-legacy.txt`](MIT-legacy.txt) |

`LICENSE` is the Free Software Foundation's GPLv3 text, unmodified, including the preamble, the terms and conditions, and the "How to Apply These Terms to Your New Programs" appendix. That appendix is part of the license document. It contains the Foundation's sample notice, which includes the words "or (at your option) any later version."

The grant for this repository is **GPL-3.0-only**: version 3 of the GNU GPL, with no later-version option. The appendix sample is the Foundation's general example. It is not an additional grant for Splatty.

## First-party scope

GPL-3.0-only applies to first-party material in this tree as published with this change and in later revisions: source, scripts, tests, and documentation written for Splatty.

`LICENSES/MIT-legacy.txt` is a preserved copy of the previous root `LICENSE` file. It records the MIT grant. Distributions of this revision are under GPL-3.0-only.

The GPLv3 text in `LICENSE` is the Free Software Foundation's license document. Its header allows verbatim copies and forbids changes to that document.

## Names already on record

This migration leaves the existing copyright line as written. It does not add an owner.

- The preserved MIT file states `Copyright (c) 2026 Near`.
- Git history for this repository is committed under the author name Near.
- The README non-goals mention Neil only for a hardware-purchase decision. That sentence is not a copyright line.

Contributors keep copyright in their own contributions. This notice does not assign that copyright to anyone else.

## MIT rights from before this change

`MIT-legacy.txt` is the previous `LICENSE` file byte for byte. It keeps the Near copyright line and the MIT permission notice, beginning "Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software")".

Anyone who received a copy of this project under that MIT license keeps the rights that copy granted. Offering this revision and later revisions under GPL-3.0-only leaves those earlier MIT grants in place. History is unchanged, so those earlier revisions still contain the MIT license. There are no tags or GitHub releases in this repository; the earlier copies are the revisions that carried the MIT `LICENSE`.

## Outside this grant

This notice does not relicense third-party material, and it does not add a third-party notice that this tree did not already contain.

- [msplat](https://github.com/rayanht/msplat) is an external training tool. `Mac/train/README.md` already records it as Apache-2.0. That sentence is unchanged. The tool is not vendored in this repository. Upstream's repository license is Apache-2.0, which matches that note.
- [MetalSplatter](https://github.com/scier/MetalSplatter) is named in the README and in `docs/architecture.md` as a planned preview renderer. Its source is not in this repository. This tree does not include MetalSplatter's license text, and this change does not add that text. Upstream remains under its own MIT license.
- The default branch has no package manifest, lockfile, vendored dependency, third-party notice file, or attributed asset.
- The [3D Gaussian Splatting](https://repo-sam.inria.fr/fungraph/3d-gaussian-splatting/) link in the README is a citation. That project is not in this tree.
- Files that arrive later with their own license or asset terms stay under those terms.
