# FuseBase Troubleshooter: corresponding source of the FFmpeg WebAssembly core

This folder holds the complete corresponding source code of the FFmpeg WebAssembly core that the FuseBase
Troubleshooter browser extension ships (4.8 and later). The extension's `THIRD_PARTY_NOTICES.txt` ("Source code
availability") links to it instead of a written offer.

Hosted at https://github.com/fusebase-dev/Fusebase-troubleshooter-extension (public repository; the hosted link is
the only source channel, with no email or written-offer contact).

Assembled 2026-09-24 (extension commit T18 in `fusebase-troubleshooter`). Verify with `sha256sum -c SHA256SUMS`.

## The shipped binary this source corresponds to

| Item | Value |
|---|---|
| Package | `@ffmpeg/core@0.12.10`, `dist/umd`, npm shasum `3177e88852bfbfaad5d258e9e0ac1fd9dffd3223`, published 2025-01-07T10:13:14Z |
| Extension files | `assets/ffmpeg/ffmpeg-core.js` sha256 `b266ab5b952555881dd6310663986994a182acb2b7ff25cf10a25f7a37ac2b21` |
| | `assets/ffmpeg/ffmpeg-core.wasm` sha256 `9f57947a5bd530d8f00c5b3f2cb2a3492faa7e5d823315342d6a8656d0a6b7b7` |
| Licence of the whole | GPL-2.0-or-later (FFmpeg configured with `--enable-gpl`, no `--enable-nonfree`) |

## Contents

Every tarball is GitHub's archive of one exact commit: its top directory is `<repo>-<full commit id>` and its
gzip/pax comment carries the same commit id.

| File in `src/` | Component | Repository | Ref in the Dockerfile | Exact commit | Licence |
|---|---|---|---|---|---|
| `ffmpeg.wasm-core-v0.12.10-release-71aa99d37c02.tar.gz` | build recipe: Dockerfile, `build/*.sh`, `src/bind`, `src/fftools` | ffmpegwasm/ffmpeg.wasm | release commit (tag `v12.15`) | `71aa99d37c02a7b4c435275ca9ef50e612f6efa1` | MIT (scripts); fftools GPL/LGPL as FFmpeg |
| `FFmpeg-n5.1.4-4729204c17f7.tar.gz` | FFmpeg | FFmpeg/FFmpeg | tag `n5.1.4` | `4729204c17f756e186d622060088371d10b34f7e` | LGPL-2.1-or-later; GPL-2.0-or-later as built |
| `x264-4-cores-33cac6b77d5b.tar.gz` | x264 | ffmpegwasm/x264 | branch `4-cores` | `33cac6b77d5b9259c552156013a817ab23119612` | GPL-2.0-or-later |
| `x265-3.4-2bb5520e9596.tar.gz` | x265 | ffmpegwasm/x265 | tag `3.4` (lightweight) | `2bb5520e9596f361bf0ed81b3b8da0d7fd999069` | GPL-2.0-or-later |
| `libvpx-v1.13.1-10b9492dcf05.tar.gz` | libvpx | ffmpegwasm/libvpx | tag `v1.13.1` | `10b9492dcf05b652e2e4b370e205bd605d421972` | BSD-3-Clause |
| `lame-master-2badea1974ae.tar.gz` | LAME 3.100 | ffmpegwasm/lame | branch `master` | `2badea1974ae36cb8312afe99cff1e6b3b5decee` | LGPL-2.0-or-later |
| `ogg-v1.3.4-bada45718453.tar.gz` | Ogg | ffmpegwasm/Ogg | tag `v1.3.4` | `bada45718453ac27b56773ae663f7e65112f6a6e` | BSD-3-Clause |
| `theora-v1.1.1-7ffd8b2ecfc2.tar.gz` | Theora | ffmpegwasm/theora | tag `v1.1.1` | `7ffd8b2ecfc2d93ae5e16028e7528e609266bfbf` | BSD-3-Clause |
| `opus-v1.3.1-e85ed7726db5.tar.gz` | Opus | ffmpegwasm/opus | tag `v1.3.1` | `e85ed7726db5d677c9c0677298ea0cb9c65bdd23` | BSD-3-Clause |
| `vorbis-v1.3.3-779816404319.tar.gz` | Vorbis | ffmpegwasm/vorbis | tag `v1.3.3` | `7798164043197d7e33f02de4353ce2aa5b248225` | BSD-3-Clause |
| `zlib-v1.2.11-cacf7f1d4e3d.tar.gz` | zlib | ffmpegwasm/zlib | tag `v1.2.11` | `cacf7f1d4e3d44d871b605da3b647f07d718623f` | Zlib |
| `libwebp-v1.3.2-ca332209cb55.tar.gz` | libwebp | ffmpegwasm/libwebp | tag `v1.3.2` | `ca332209cb5567c9b249c86788cb2dbf8847e760` | BSD-3-Clause |
| `freetype2-VER-2-10-4-6a2b3e4007e7.tar.gz` | FreeType | ffmpegwasm/freetype2 | tag `VER-2-10-4` | `6a2b3e4007e794bfc6c91030d0ed987f925164a8` | FTL or GPL-2.0 |
| `fribidi-v1.0.9-f9e8e71a6fbf.tar.gz` | FriBidi | fribidi/fribidi | tag `v1.0.9` | `f9e8e71a6fbf4a4619481284c9f484d10e559995` | LGPL-2.1-or-later |
| `harfbuzz-5.2.0-4a1d891c6317.tar.gz` | HarfBuzz | harfbuzz/harfbuzz | tag `5.2.0` | `4a1d891c6317d2c83e5f3c2607ec5f5ccedffcde` | MIT |
| `libass-0.15.0-d149636f502f.tar.gz` | libass | libass/libass | tag `0.15.0` | `d149636f502f5774ae1a8fb4c554b122674393b2` | ISC |
| `zimg-release-3.0.5-e5b0de6bebbc.tar.gz` | zimg | sekrit-twc/zimg | tag `release-3.0.5` | `e5b0de6bebbcbc66732ed5afaafef6b2c7dfef87` | WTFPL |
| `emscripten-3.1.40-5c27e79dd0a9.tar.gz` | Emscripten 3.1.40: its system libraries (libc, libc++, compiler-rt) are linked into the wasm | emscripten-core/emscripten | tag `3.1.40` (image `emscripten/emsdk:3.1.40`) | `5c27e79dd0a9c4e27ef2326841698cdd4f6b5784` | MIT / NCSA, and the licences in its `system/lib` |
| `SDL2-release-2.24.2-emscripten-port.zip` | SDL2 port that `-sUSE_SDL=2` makes available (no SDL code observed in the binary; included to be safe) | libsdl-org/SDL | tag `release-2.24.2`, pinned by sha512 in Emscripten 3.1.40 `tools/ports/sdl2.py` | `55b03c7493a7abed33cf803d1380a40fa8af903f` | Zlib |

`extra/ffmpeg.wasm-v0.12.10-c3a763857c5e.tar.gz` is ffmpeg.wasm tag `v0.12.10` (commit `c3a7638`, 2023-12-25).
It is NOT the core's source: that tag is the `@ffmpeg/ffmpeg` 0.12.10 wrapper release, where `packages/core` is still
0.12.6 and the build scripts lack the `ffprobe` export and `-sENVIRONMENT=worker` that the shipped `ffmpeg-core.js`
has. Earlier notices pointed at it; it is kept for comparison only. Do not host it as the corresponding source.

`evidence/` holds the proof: `provenance.json` (every pin and why), `github-ref-activity.json` (GitHub ref activity
per pinned ref), `wasm-version-strings.txt` (version markers read from the shipped wasm), `Dockerfile-71aa99d`.

## How each pin was proven

| Pin | Proof |
|---|---|
| ffmpeg.wasm `71aa99d` | It is the commit "RELEASE: @ffmpeg/core and @ffmpeg/core-mt v0.12.10" (2025-01-07T10:12:48Z, 26 s before the npm publish); its `packages/core/package.json` is 0.12.10. The shipped `ffmpeg-core.js` exports `_ffprobe` and runs worker-only, which the build scripts produce only from `bd903bb` (2024-08-30) on; `c3a7638` lacks both. Build inputs (`build/`, `src/fftools`, `src/bind`) last changed 2024-08-30 (`bd903bb`); the Dockerfile last changed 2023-12-25 (`e0d4c62`) |
| Tags (FFmpeg, x265, libvpx, Ogg, Theora, Opus, Vorbis, zlib, libwebp, FreeType, FriBidi, HarfBuzz, libass, zimg, Emscripten, SDL) | `git ls-remote` resolves each tag to the commit above. GitHub's repository activity API records no change to any of these refs since its retention start (entries back to 2023-03 are visible on ffmpeg.wasm); FFmpeg `n5.1.4` shows one tag event on 2023-11-10, before the build. Binary markers agree: `5.1.4` and `Lavc59.37.100` (FFmpeg), `WebM Project VP8/VP9 Encoder v1.13.1` (libvpx), `FriBidi 1.0.9`, `Xiph.Org libtheora 1.1`, LAME `3.100` |
| x264 branch `4-cores` = `33cac6b` | Head today; committed 2022-08-22, the only commit on the branch beyond upstream `baee400`. GitHub activity: no push, force-push or ref change on this repository since retention start (2023). Every build of the 0.12.10 Dockerfile runs on `emsdk:3.1.40` + `FFMPEG_VERSION=n5.1.4` (set 2023-12-17), so the branch was resolved after 2023-12-17, inside the window with no ref change. The wasm says `x264 - core 0000` (built without `.git`, so no commit id is embedded) and copyright 2003-2022 |
| LAME branch `master` = `2badea1` | Head today and the only commit ("Init commit with lame 3.100", 2020-10-29); no activity since retention start; the wasm carries LAME `3.100` |
| x265 tag `3.4` = `2bb5520` | Lightweight tag, commit 2020-05-29; no activity since retention start |

## Limits (not proven)

- Where the binary was built is unknown (no CI log; Inferred: a maintainer build, since the release is a manual
  "RELEASE" commit). That the npm bytes rebuild from these sources was not tested (no Docker rebuild was run).
- GitHub's activity record starts around 2023; a ref change before that is invisible, but it cannot affect a build
  that resolved the refs after 2023-12-17.
- Docker `ADD <git>#<ref>` resolves refs at build time and the builder's cache state is unknown; the argument
  above rests on the base-layer change of 2023-12-17 invalidating older cached layers (Inferred from Docker layer
  caching, not observed).

## Not included (not part of the corresponding source)

- Toolchain binaries from the `emscripten/emsdk:3.1.40` image (LLVM, Binaryen, Node): compilers, not linked in.
- Test-only git submodules: ffmpeg.wasm `testdata`, zimg `test/extra/googletest`, Emscripten test suites.
- `@ffmpeg/ffmpeg` 0.12.15 (the MIT wrapper `ffmpeg.js` / `814.ffmpeg.js`): MIT, no source obligation.

## Rebuilding

Unpack `src/ffmpeg.wasm-core-v0.12.10-release-71aa99d37c02.tar.gz` and run `make prd` (the single-thread production
build: `docker buildx build` with `FFMPEG_ST=yes` and `EXTRA_CFLAGS="-O3 -msimd128"`, output in `packages/core/dist`).
The Dockerfile fetches each component by ref over the network; to build offline, replace each `ADD https://github.com/...#<ref> /src` with the matching
tarball from `src/` (and the zimg `git clone` likewise).
