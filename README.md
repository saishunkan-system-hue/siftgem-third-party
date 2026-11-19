# SiftGem — third-party corresponding source

This repository exists to satisfy one obligation. Some components shipped with
SiftGem are licensed under the GNU GPL or LGPL, which require that the
corresponding source code be made available to anyone who has the binaries.
`compliance/THIRD-PARTY-NOTICES.txt`, delivered with every copy of the product,
makes a written offer in its section 3.0 and points here.

It holds **third-party source only**. None of SiftGem's own source is here.

## There is no single licence for this repository

Do not read one. Every archive here carries the licence its own author chose --
GPL-2.0, GPL-3.0, LGPL-2.1, BSD, MIT, Apache-2.0 and many more across the
2,210 files published under each tag. No file at the root of this
repository grants you anything, and none purports to: whoever published this has
no right to relicense other people's work, and has not tried to.

`licenses/` republishes the few licence texts the product itself carries beside
its manifests: poppler's GPL-2.0 and GPL-3.0 texts (with its Debian copyright
file, where the build has one), Redis's BSD-3-Clause licence and the licences
of the libraries Redis bundles. It is not a collection of every licence
involved, and it is not where the LGPL texts are. For any individual archive,
the authoritative licence is the one inside that archive, and `manifests/`
records the licence each package declared when it was collected.

## Finding the source for your machine

Open `compliance/THIRD-PARTY-NOTICES.txt` on the machine and read the
`Delivered build` line at the top of the document. That string is a git tag in
this repository. Everything published under that tag is the corresponding
source for that build, and nothing else is.

SiftGem runs on two processor architectures. Take the set for yours: `arm64`
for a Mac with Apple Silicon, `amd64` for Windows, Intel or other x86 machines.
`uname -m` prints `arm64`/`aarch64` or `x86_64`.

This build: **`v1.0.1`**

## What is where

| | |
|---|---|
| `components/` | source for components shipped as binaries that are not operating-system packages (gcc-runtime, keyutils-1.5.8-3.el7.src.rpm, opencv-contrib-python-4.10.0.84, opencv-contrib-python-4.10.0.84-linux, opencv-python-5.0.0.93, shapely-geos) |
| `manifests/` | every archive named with the checksum it was verified against |
| `licenses/` | the licence texts the product carries for poppler and Redis; every other archive carries its own |
| Release assets | the operating-system source, per architecture, listed below |

The release attached to this tag carries:

* `os-arm64-v1.0.1.tar` (1,602 MB, 1,057 files) — operating-system source for arm64 (section 3.2)
* `os-amd64-v1.0.1.tar` (1,680 MB, 1,079 files) — operating-system source for amd64 (section 3.2)
* `components-large-v1.0.1.tar` (131 MB) — files of `components/` too large for git, at the same paths; listed in `manifests/components-MANIFEST.txt`

They are plain `.tar`; the files inside are already compressed. Where one
architecture's set is split into parts, extract every part into the same
directory.

## Verifying what you download

Do not take these bytes on trust, including from us. Every archive is listed in
a manifest with a SHA-256:

* `manifests/os-arm64-MANIFEST.txt` — every operating-system source archive for arm64, with the checksum its own publisher recorded and its SHA-256 as published here.
* `manifests/os-amd64-MANIFEST.txt` — every operating-system source archive for amd64, with the checksum its own publisher recorded and its SHA-256 as published here.
* `manifests/components-MANIFEST.txt` — every archive under `components/` with its SHA-256.

Copies of these manifests also travel with the product itself, under
`compliance/third-party-source/`, so you can check what you download here
against something that arrived with your machine rather than against this
server.

## If this repository is unreachable

The offer in section 3.0 stands regardless. Write to the address in that
section and a copy will be sent on physical media at cost.
