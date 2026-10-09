# Fork provenance and redistribution guardrails

**Repository:** [DataRaul/rea](https://github.com/DataRaul/rea)  
**Original project:** [morluto/rea](https://github.com/morluto/rea)  
**Recorded fork baseline:** `392f1f310733f2c365da7bc57a1154cf10ec4ba0` (2026-10-09)  
**Scope:** Provenance and operational checklist, not a comprehensive legal or dependency audit.

## Core source and attribution

- REA's root [LICENSE](LICENSE) is MIT, bearing `Copyright (c) 2026 morluto`. **Retain this original copyright and permission notice** in redistributed copies or substantial portions, including any derivative packaging where required.
- A GitHub fork is not an assertion that the original author endorses this fork. Do not use the upstream identity to imply endorsement.
- Keep the original authorship/history intact. Clearly identify substantive local modifications if any are made.
- Follow the upstream [AGENTS.md](AGENTS.md) and [CONTRIBUTING.md](CONTRIBUTING.md) before changing runtime code.

## Third-party boundaries

- The [submodule manifest](.gitmodules) references `jadx-headless-mcp`, `binwalk`, `unblob`, `ghidra-nativeaot`, and `wakaru`. Submodule pointers are not blanket permission to relicense or redistribute those projects. Review each **pinned** revision's license/notice obligations before redistributing its source or binary.
- [third_party/README.md](third_party/README.md) documents REA's externally supplied analysis engines, including JADX (Apache-2.0) and Binwalk/Unblob (MIT).
- Local notice files for the EVMole dependency ([third_party/evmole/LICENSE](third_party/evmole/LICENSE)) and pwndbg ([third_party/pwndbg/LICENSE.md](third_party/pwndbg/LICENSE.md)) must remain intact in copies containing those materials.
- Other runtime/build dependencies, generated builds and platform-specific tools may carry separate terms. **This checklist does not establish a complete software-bill-of-materials license clearance.** No bundled artifacts or published package have been audited here.

## Responsible use and downstream integration

- Investigate only software and data for which the operator has appropriate authorization. A permissive license on REA **does not** grant rights to target software, datasets, authentication systems, or services.
- Respect applicable law, privacy and access controls; do not bypass protections or collect secrets. Review target-specific terms before automated inspection.
- Treat this repository as an **independent optional tool**. Future Agent OS use must be explicit, version-pinned, bounded, read-only by default, and operator-approved for any target inspection or local setup. No Agent OS integration or runtime activation is authorized by this note.
- No paid providers, external target analysis, or GitHub Actions are required to maintain this fork's legal provenance.

## Maintenance checklist

1. When synchronizing upstream, record the new source commit and review changes to `LICENSE`, `.gitmodules`, `third_party/`, packaging, and download/setup behavior.
2. Preserve required copyright, license and third-party notices. Review any new vendored files, binaries or distributions separately before redistribution.
3. If local changes are published, describe them accurately without presenting the fork as the upstream release.
4. Validate an actual runtime/integration separately; a source-code fork is **not** proof that installation or analysis functionality works.

This file records a limited factual review of the source tree on 2026-10-09, not legal advice or a certification of every dependency.
