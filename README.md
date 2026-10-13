# cadcraft-ko-patch

Korean (한국어) interface patch for **[CADCraft](https://github.com/storytold/cadcraft)** (AutoCAD-class CAD/drafting), upstream tag `v0.6.2`.
This repository contains **only the patch**, not CADCraft's source code. See `BASE.txt` for the exact upstream commit.

## Apply
```bash
git clone --branch v0.6.2 https://github.com/storytold/cadcraft.git && cd cadcraft
git apply ../cadcraft-ko-patch/patches/cadcraft-v0.6.2-ko.patch
```
Then build as upstream documents. Windows build without MSVC: [artcraft-ko-toolkit](https://github.com/lubydubybubu/artcraft-ko-toolkit).

## What it changes
Korean catalog ported from storytold/cadcraft PR #857 (huk082): 1,177 rows unchanged, 58 revised to Korean AutoCAD wording (합니다체 messages, 테이블, 대칭, 직교 모드 …; Layer stays 도면층 as in the Korean AutoCAD edition); Malgun Gothic font search on Windows.
Changed files: `CHANGED-FILES.txt`.

## Verified
Korean 10/10 (RED first), i18n 27, theme 4 on Linux.

## Known limits
Korean font tests skip on machines without a Hangul font.

Translations are AI-assisted (Claude Opus 5.5) and not reviewed by a professional translator.
Licence: MIT OR Apache-2.0, same as CADCraft; upstream contributions credited above.
