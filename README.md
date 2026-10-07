# Odoo Addon Migrator — Releases

Public desktop releases for **Odoo Addon Migrator**.

Current corrected releases: **[Windows v1.0.5](https://github.com/UsamaFathi/Odoo-Addon-Migrator-Releases/releases/tag/v1.0.5-windows)** and **[Ubuntu v1.0.5](https://github.com/UsamaFathi/Odoo-Addon-Migrator-Releases/releases/tag/v1.0.5-ubuntu)**.

The latest rebuild fixes Odoo 19 search-view group attributes and legacy `attrs` conversion, and retains the earlier folder-selection fix. The trained Brain is unchanged; **no retraining is required**. Download fresh files, reinstall and rerun migration into a new output folder. The displayed version remains 1.0.5; manifests identify the new build as `search-group-attributes-fix`.

The Windows v1.0.5 installer and portable ZIP are rebuilt, tested and published. The folder-selection cache no longer requires loose Python source files.

Odoo Addon Migrator helps developers migrate custom Odoo addons across supported versions from **Odoo 14 through Odoo 19** while keeping the original addon folder unchanged.

The Windows and Ubuntu v1.0.5 desktop packages include **Community migration knowledge**. Enterprise overlays remain separate artifacts for local authorized use and are not distributed in this release. End users select only their custom addons and migration versions; no Odoo source checkout, Enterprise source folder, training step, or runtime source indexing is required.

The public desktop interface is intentionally simplified: Official Odoo source management, Community/Enterprise source paths, and Migration Brain controls are not exposed to end users. The Project page remains clean and scrollable while the bundled migration knowledge works internally.

The packaged migration knowledge contains derived compatibility data only and does not contain Odoo Community or Enterprise source files.

## Current release status

Windows v1.0.5 adds structural View Intelligence with a retrained schema-v5 Community Brain. It analyzes moved, hidden, replaced and fragile inherited-view anchors and suggests candidates for review without speculative XML replacement. Canonical source support does not prove effective database view compatibility. Historical release notes remain in this repository.

Ubuntu v1.0.5 uses the identical Community Brain. All 280 tests passed on both platforms; isolated installation, offscreen/X11 GUI startup and removal were verified in Ubuntu 22.04.5. The Windows installer and portable folder-selection smoke tests passed as well.

[Download Ubuntu v1.0.5](https://github.com/UsamaFathi/Odoo-Addon-Migrator-Releases/releases/tag/v1.0.5-ubuntu). Tested in a 4 GB VM; 8 GB RAM is recommended. A 2 GB VM was insufficient. See its release notes for CPU requirements and measured startup memory/time.

## Downloads

Corrected Windows and Ubuntu packages use separate release tags.

### Windows release

[Download corrected Windows v1.0.5](https://github.com/UsamaFathi/Odoo-Addon-Migrator-Releases/releases/tag/v1.0.5-windows)

- `OdooAddonMigrator_Setup.exe` ? installer; close the app and reinstall.
- `OdooAddonMigrator-Windows.zip` ? portable application.
- `SHA256SUMS-Windows.txt` and `release-manifest.json` ? checksums and validation.

### Ubuntu x86_64 release

Release tag format:

`v<version>-ubuntu`

For v1.0.5:

`v1.0.5-ubuntu`

Assets:

- `OdooAddonMigrator_1.0.5_amd64.deb` — recommended Ubuntu package.
- `OdooAddonMigrator-Ubuntu-x86_64.tar.gz` ? portable application.
- `SHA256SUMS-Ubuntu.txt` and `release-manifest-ubuntu.json` ? checksums and validation.

Install the Debian package with:

```bash
sudo apt install ./OdooAddonMigrator_1.0.5_amd64.deb
```

## What is bundled

Windows and Ubuntu v1.0.5 include:

- Community migration knowledge for Odoo 14 through Odoo 19.
- The desktop migration engine and static validation workflow.

The v1.0.5 build verifies the Community Brain integrity and excludes Enterprise overlays. Older release notes describe the contents of their respective packages.

## Typical workflow

1. Select the custom addons folder.
2. Confirm or choose the source Odoo version.
3. Choose the target Odoo version.
4. Choose a separate output folder.
5. Start the migration.
6. Review the migration report and diff.
7. Install and test the migrated addons on the target Odoo environment.

There is no source-management setup step in the public app.

The original custom addon folder is not modified by the migration workflow.

## Feedback and bug reports

We are actively collecting real migration experience to improve compatibility and usability.

Use the repository **Issues** section and choose:

- **Bug report** for crashes, installation problems, incorrect migrations, or validation problems.
- **Product feedback** to share migration results, manual fixes that were still required, and UI/workflow feedback.

Please do **not** post credentials, customer data, proprietary addon source code, private logs containing secrets, or other sensitive information in public issues.

## Validation and production use

Static migration and validation cannot guarantee production compatibility. Always install and test migrated addons on the target Odoo version before using them in production.

The Windows installer may be unsigned, so Microsoft SmartScreen can display a warning.

## Checksums

Stable releases include SHA-256 checksum files so downloaded files can be verified before installation.

## Project note

This repository contains public release files and feedback resources only. Application development is maintained separately.

Odoo Addon Migrator is an independent migration utility and is not affiliated with Odoo S.A.
