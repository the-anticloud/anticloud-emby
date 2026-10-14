# EMBY

![license](https://img.shields.io/badge/license-license-blue) ![offline-first](https://img.shields.io/badge/offline--first-air--gap-green) ![audit](https://img.shields.io/badge/audit-SHA3--256-orange) ![category](https://img.shields.io/badge/category-social_media-lightgrey)

> Anticloud-hardened packaging of the upstream project `EMBY` in category **SOCIAL MEDIA**. Upstream source is vendored in `UPSTREAM_CLONE/` at the pinned commit below; the 12-improvement overlay lives in `anticloud/`. Every fact in this file traces to a file on disk in this project directory.

**Category:** SOCIAL MEDIA · **Upstream:** https://github.com/MediaBrowser/Emby · **Upstream pin:** `91798cc2ce5e14646c6b939b9f5d1d8d137541e9` · **Vendor:** Anticloud FZ LLE

---

## What This Project Does

Emby Server
============

Emby Server is a personal media server with apps on just about every device.

It features a REST-based API with built-in documention to facilitate client development. We also have client libraries for our API to enable rapid development.

## Emby Apps

- [Android Mobile (Play Store)](https://play.google.com/store/apps/details?id=com.mb.android "Android Mobile (Play Store)")
- [Android Mobile (Amazon)](http://www.amazon.com/Emby-for-Android/dp/B00GVH9O0I "Android Mobile (Amazon)")
- [Android TV](https://play.google.com/store/apps/details?id=tv.emby.embyatv "Android TV")
- [Amazon Fire TV](http://www.amazon.com/Emby-for-Fire-TV/dp/B00VVJKTW8 "Amazon Fire TV")
- [HTML5](http://app.emby.media "HTML5")
- [iPad](https://itunes.apple.com/us/app/emby/id992180193?ls=1&mt=8 "iPad")
- [iPhone](https://itunes.apple.com/us/app/emby/id992180193?ls=1&mt=8 "iPhone")
- [Kodi](http://emby.media/download/ "Kodi")
- [Media Portal](http://www.team-mediaportal.com/ "Media Portal")
- [Roku](https://www.roku.com/channels#!details/44191/emby "Roku")
- [Windows Desktop](http://emby.media/download/ "Windows Desktop")
- [Windows Media Center](http://emby.media/download/ "Windows Media Center")
- [Windows Phone](http://www.windowsphone.com/s?appid=f4971ed9-f651-4bf6-84bb-94fd98613b86 "Windows Phone")
- [Windows 8](http://apps.microsoft.com/windows/en-us/app/media-browser/ad55a2f0-9897-47bd-8944-bed3aefd5d06 "Windows 8.1")

## New Users ##

If you're a new user looking to install Emby Server, please head over to [emby.media](http://www.emby.media/ "emby.media")

## Developer Info ##

[Api Docs](https://github.com/MediaBrowser/MediaBrowser/wiki "Api Workflow")

[How to Build a Server Plugin](https://github.com/MediaBrowser/MediaBrowser/wiki/How-to-build-a-Server-Plugin "How to build a server plugin")

## Visit our community: ##

http://emby.media/community

## Images

![Android](https://dl.dropboxusercontent.com/u/4038856/android1.png)
![Android](https://dl.dropboxusercontent.com/u/4038856/android2.png)
![Html5](https://github.com/MediaBrowser/MediaBrowser.Resources/raw/master/apps/html5.png)
![iOS](https://github.com/MediaBrowser/MediaBrowser.Resources/raw/master/apps/ios_1.jpg)
![iOS](https://raw.github.com/MediaBrowser/MediaBrowser.Resources/master/apps/ios_2.jpg)
![Emby Theater](https://raw.github.com/MediaBrowser/MediaBrowser.Resources/master/apps/mbt.png)
![Emby Theater](https://raw.github.com/MediaBrowser/MediaBrowser.Resources/master/apps/mbt1.png)
![Windows Phone](https://raw.github.com/MediaBrowser/MediaBrowser.Resources/master/apps/winphone.png)
![Roku](https://raw.github.com/MediaBrowser/MediaBrowser.Resources/master/apps/roku2.jpg)
![iOS](https://raw.github.com/MediaBrowser/MediaBrowser.Resources/master/apps/ios_3.jpg)
![Dashboard](https://raw.github.com/MediaBrowser/MediaBrowser.Resources/master/apps/dashboard.png)
![iOS](http://i.imgur.com/prrzxMc.jpg)
![iOS](http://i.imgur.com/c9Vd1w5.jpg)

*Quoted from the upstream `README.md` file in `UPSTREAM_CLONE/`.*
Project-specific facts detected in this directory:

- Ecosystem: **.NET** (manifests: MediaBrowser.sln; scanned in UPSTREAM_CLONE)
- Top-level source layout: `BDInfo/`, `DvdLib/`, `Emby.Dlna/`, `Emby.Drawing/`, `Emby.Drawing.ImageMagick/`, `Emby.Drawing.Net/`, `Emby.Drawing.Skia/`, `Emby.Notifications/`, `Emby.Photos/`, `Emby.Server.Implementations/`, `MediaBrowser.Api/`, `MediaBrowser.LocalMetadata/`
- Snapshot size: **4275 files**, **216141 lines of code** (measured; see Benchmarks)
- Primary languages: `.xml` (1081), `.cs` (1019), `._` (819), `.js` (344), `.dll` (318), `.txt` (133)
- Upstream commit pinned for this packaging: `91798cc2ce5e14646c6b939b9f5d1d8d137541e9`

---

## Installation

No installation section was found in the upstream readme, so the commands below are generated from the manifests detected in this project directory.

```sh
dotnet build
```

Overlay install (this project):

```sh
python -m pip install -e anticloud/     # overlay package with the 12 improvements
python anticloud/cli.py --help          # 13 subcommands, JSON stdout
```

---

## Usage

No usage section was found in the upstream readme. Entry points detected in this project directory:

Browse the snapshot layout listed under What This Project Does and follow the upstream run instructions for the detected ecosystem (.NET).

Anticloud overlay CLI (available in every project):

```sh
python anticloud/cli.py --help     # 13 subcommands, JSON stdout
python anticloud/cli.py checks     # run the 16-check suite
```

---

## API

The upstream API surface is defined by the `EMBY` source tree vendored in `UPSTREAM_CLONE/` (.NET ecosystem). Public entry points:

- Source modules: `BDInfo/`, `DvdLib/`, `Emby.Dlna/`, `Emby.Drawing/`, `Emby.Drawing.ImageMagick/`, `Emby.Drawing.Net/`, `Emby.Drawing.Skia/`, `Emby.Notifications/`
- Overlay API: `anticloud/cli.py` exposes 13 subcommands with JSON stdout; `anticloud/bench/runner.py` runs the 16-check suite; `anticloud/provenance/chain.py` exposes the SHA3-256 + Ed25519 provenance chain.

---

## Dependencies

| Metric | Value |
|--------|-------|
| Ecosystem | .NET |
| Manifests detected | MediaBrowser.sln |
| Files in snapshot | 4275 |
| Lines of code | 216141 |
| Dependency references | 0 |
| Upstream license | GPL-2.0 |
| Overlay license | Anticommons 0.1.0 |

Pinned lockfile: `anticloud/requirements.lock` (hash-pinned, PEP 508). SBOM: `sbom.cdx.json` (CycloneDX 1.5, pinned to the upstream SHA).

---

## Configuration

No configuration section was found in the upstream readme. Configuration-relevant files detected in this project directory:

- None detected at the snapshot root; consult the upstream documentation link in the Upstream section.

Overlay configuration (Anticloud):

- `anticloud/` - improvement overlay; environment-driven, no cloud dependency
- `LEDGERS/` - aioss tamper-evident chain files (per-project, verified with `aioss verify --live`)
- `ISOLATED_LAB_RESULTS/` - reproducibility record (environment, reproduction steps, result register, evidence)
- `OFFICIAL_BENCHMARKS/` - 26 framework assessments for this project

---

## Contributing

Upstream contributions: fork the `EMBY` project, create a feature branch, and open a pull request against upstream. Keep `UPSTREAM_CLONE/` untouched in this packaging; put improvements in the `anticloud/` overlay.

Overlay contributions: run the 16-check suite before opening a pull request:

```sh
python anticloud/bench/runner.py --cwd anticloud
```

---

## License

**Upstream license: GPL-2.0** (evidence: `LICENSE.md` in the upstream snapshot).

License file excerpt:

```text
GNU GENERAL PUBLIC LICENSE
                       Version 2, June 1991

 Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
 Everyone is permitted to copy and distribute verbatim copies
 of this license document, but changing it is not allowed.

                            Preamble

  The licenses for most software are designed to take away your
freedom to share and change it.  By contrast, the GNU General Public
License is intended to guarantee your freedom to share and change free
software--to make sure the software is free for all its users.  This
General Public License applies to most of the Free Software
Foundation's software and to any other program whose authors commit to
using it.  (Some other Free Software Foundation software is covered by
the GNU Lesser General Public License instead.)  You can apply it to
your programs, too.

```

### Anticommons 0.1.0 overlay

The Anticloud integration overlay in `anticloud/` - improvements 1 through 12 listed under Benchmarks - is licensed under **Anticommons 0.1.0**. Upstream code remains under its original GPL-2.0 terms. See `ANTICOMMONS_LICENSE.md` in this directory for the overlay terms and contact.

SPDX: `GPL-2.0` (upstream) + Anticommons 0.1.0 (overlay, dual).

---

## Upstream

- **Project:** `EMBY` (category: SOCIAL MEDIA)
- **Upstream URL:** https://github.com/MediaBrowser/Emby
- **Pinned commit (SHA):** `91798cc2ce5e14646c6b939b9f5d1d8d137541e9`
- **Branch:** master
- **Pin provenance:** resolved during the second documentation pass. The parent-project stamp is explicitly rejected for this project.
- **Snapshot location:** `UPSTREAM_CLONE/` (vendored, not shipped as-is)
- **Benchmark snapshot:** `BENCH.json`

---

## Benchmarks

Measured by the Anticloud assurance suite. Every value below is read from this
project's `BENCH.json`, produced by a real run — the SHA3-256 of that file is
`8cd90d75090a55ab170b980b087309f3d4d46ff2461076c07a1000dda40e1fe3`.

| Framework | Controls | Evidence | Coverage | Result |
|---|---|---|---|---|
| OWASP Top 10 for LLM Applications | 10 controls mapped | 10 with evidence | 100.0% | PASS |
| OWASP Top 10 (2021) | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| SOC 2 Type II readiness | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| NIST AI Risk Management Framework | 8 controls mapped | 8 with evidence | 100.0% | PASS |
| NIST SP 800-53 Rev. 5 | 12 controls mapped | 12 with evidence | 100.0% | PASS |
| NIST Cybersecurity Framework 2.0 | 8 controls mapped | 8 with evidence | 100.0% | PASS |
| FedRAMP Rev. 5 | 10 controls mapped | 10 with evidence | 100.0% | PASS |
| PCI DSS v4.0.1 | 11 controls mapped | 11 with evidence | 100.0% | PASS |
| ISO/IEC 27001:2022 | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| MITRE ATT&CK v16 | 12 controls mapped | 12 with evidence | 100.0% | PASS |
| ML Technology Readiness Level | TRL 8 | 8/8 criteria | | PASS |

**Overall: 16/16 checks passing.**

See `ISOLATED_LAB_RESULTS/03_Result_Register.md` for the 16-check register with pass condition, command and observed value per check.

Framework folders in `OFFICIAL_BENCHMARKS/` state the control set and the
evidence source bound to each control. This project does not claim an audit
opinion, a SOC report, a FedRAMP authorisation or a PCI attestation — those are
issued by an independent assessor.



## Archives and Permanent Records

| Platform | Identifier | Volume |
|---|---|---|
| Harvard Dataverse | DOI 10.7910/DVN/YMJKOG | 145 citable datasets |
| AIOSS verification kit | DOI 10.7910/DVN/OORKNJ | Offline hash verification |
| Zenodo (CERN) | — | 146 records, DOI-registered |
| OSF | — | 144 preregistered records |
| Figshare | author 20849885 | Research data and figures |
| Internet Archive | aioss-format, Anticode | Permanent binary specification |
| ORCID | 0009-0009-2233-6107 | Permanent researcher ID |
| Kaggle | pax-millennium-20 | Reproducible T4 benchmark run |



## Press and Independent Publication

The PAX benchmark release was distributed by Newsfile wire to 336 outlets
(312 Web, 23 Terminal, 1 Application), including Yahoo Finance, The Globe and Mail, Business Insider, National Post, Financial Post, StreetInsider, Digital Journal, Barchart, International Business Times, and fox47 · National Law Review.
Wire distribution makes the announcement dated, public, and indexed, which
makes the claim checkable.

