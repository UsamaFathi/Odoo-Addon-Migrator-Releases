# Odoo Addon Migrator — Releases

Public desktop releases for Odoo Addon Migrator, an independent migration utility
for custom addons across **Odoo 14 → 15 → 16 → 17 → 18 → 19**.

## Download v1.0.6

- **[Windows installer](https://github.com/UsamaFathi/Odoo-Addon-Migrator-Releases/releases/download/v1.0.6-windows/OdooAddonMigrator_Setup.exe)**
- **[Ubuntu x86_64 installer](https://github.com/UsamaFathi/Odoo-Addon-Migrator-Releases/releases/download/v1.0.6-ubuntu/OdooAddonMigrator_1.0.6_amd64.deb)**

[Windows release](https://github.com/UsamaFathi/Odoo-Addon-Migrator-Releases/releases/tag/v1.0.6-windows)
· [Ubuntu release](https://github.com/UsamaFathi/Odoo-Addon-Migrator-Releases/releases/tag/v1.0.6-ubuntu)

**v1.0.6 is installer-only.** No portable ZIP or tarball is published. Close the
application before installing the Windows update. The Windows installer also
retires stale application package metadata from previous versions.

```bash
sudo apt install ./OdooAddonMigrator_1.0.6_amd64.deb
odoo-addon-migrator
```

Ubuntu was validated on 22.04.5 x86_64, including installed offscreen/X11 startup
and removal. SSSE3, SSE4.1, SSE4.2 and POPCNT CPU support is required by bundled Qt.
8 GB RAM is recommended; earlier acceptance required a 4 GB VM. Startup loads and
verifies the Brain and can take time. Windows acceptance used an isolated test
installation and preserved the existing user installation.

## What changed

- Python window-action `tree` view types now become `list` at the 17→18 step,
  including composed upgrades to Odoo 19.
- Model-proven method references have broader coverage; unknown aliases,
  dynamic references, private RPC targets and behavior changes remain for review.
- Newly trained schema-v5 Community Brain: 210,564 examples, 17,319 view profiles
  and 84,699 anchor transitions.
- Existing settings-layout, search-view, attrs, addon identity and folder-scan
  corrections remain included.

All **363 application tests passed on each platform**. Installer startup/removal,
bundled Brain integrity and the packaged runtime modules were checked. Training
regressions passed 220 tests. Actual Odoo install-corpus validation was NOT_RUN.

Python rename calibration is deliberately conservative and small: 7 accepted
decisions from 29 trusted held-out groups, with zero observed false suggestions
and 24.14% coverage. The 18→19 slice accepted 1 of 5. Git-history supervision was
not enabled in this run. These figures do not establish support for every method
rename or business-runtime compatibility. See the platform release notes and
manifests for validation details.

## Normal use

1. Select your custom addon or containing addons directory.
2. Choose its actual original Odoo version and the higher target version.
3. Choose a fresh, separate output directory and start migration.
4. Confirm the intended technical addon name if prompted.
5. Review the report/diff and test the migrated addon in target Odoo.

Single-addon output contains a named addon folder; use its parent as the addons
path. The original addon tree is not modified. End users do not need Python,
official Odoo sources, training setup or CUDA to run the desktop tool.

Public packages contain **Community-derived knowledge only**. Enterprise overlays
remain separate, local-authorized artifacts and are not distributed. Packs contain
derived facts/model parameters, not raw Odoo source files. View suggestions are
review-only; canonical source support does not prove effective database views.

## Checksums and history

[SHA256 checksums](SHA256SUMS-v1.0.6.txt) ·
[Windows notes](RELEASE_NOTES_v1.0.6.md) ·
[Ubuntu notes](RELEASE_NOTES_v1.0.6_UBUNTU.md)

Historical [Windows v1.0.5 notes](RELEASE_NOTES_v1.0.5.md) and
[Ubuntu v1.0.5 notes](RELEASE_NOTES_v1.0.5_UBUNTU.md) remain in this repository.

## Feedback

Use Issues for bug reports or product feedback. Do not post credentials, customer
data, proprietary addon source, Enterprise source or private logs publicly.
Static validation is not production compatibility proof; install-test and exercise
business actions before deployment. The Windows installer may be unsigned and
Microsoft SmartScreen may display a warning.

This repository contains public release files and feedback resources. Application
development is maintained separately. Not affiliated with Odoo S.A.
