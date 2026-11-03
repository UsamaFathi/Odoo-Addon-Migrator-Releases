# Odoo Addon Migrator

Desktop migration assistant for custom Odoo addons, supporting forward upgrades along Odoo 14 -> 15 -> 16 -> 17 -> 18 -> 19.

## Download v1.0.7

| Platform | Installer | Tested environment |
|---|---|---|
| Windows x86_64 | [Download Windows installer](https://github.com/UsamaFathi/Odoo-Addon-Migrator-Releases/releases/download/v1.0.7-windows/OdooAddonMigrator_Setup.exe) | Windows, Python 3.12 bundled |
| Ubuntu x86_64 | [Download Debian installer](https://github.com/UsamaFathi/Odoo-Addon-Migrator-Releases/releases/download/v1.0.7-ubuntu/OdooAddonMigrator_1.0.7_amd64.deb) | Ubuntu 22.04.5 LTS |

Each release has one installer asset. No portable ZIP or tarball is published. Existing 1.0.6 releases remain available in [release history](https://github.com/UsamaFathi/Odoo-Addon-Migrator-Releases/releases).

## Changes in 1.0.7

- Newly trained, source-free schema-v6 Community Brain.
- 85 guarded review cases, 43 contextual mappings and 35 POS method suggestions.
- Conservative import/API, aggregation metadata, explicit view type, unlimited cron, plain kanban and route-declaration corrections.
- Structural view evolution and XPath risk analysis, with ambiguous suggestions kept for review.
- Semantic safeguards for HR redesigns, effective group membership, manual stock descriptions and business-specific POS changes.
- Includes earlier folder handling, Python tree/list actions, settings views, column visibility and chatter fixes.

The 85 report cases are review knowledge, not 85 automatic business-logic ports. The tool preserves the original addon tree and writes a separate output with a report and diff.

## Install and use

Windows: run the setup executable, launch the application, select the original addons folder and the actual source/target versions, then migrate into a separate destination. Keep the complete installed application directory intact.

Ubuntu:

```bash
sudo apt install ./OdooAddonMigrator_1.0.7_amd64.deb
odoo-addon-migrator
```

End users do not need Python, official Odoo sources, training setup or CUDA. Public installers contain only Community-derived facts/model parameters. Enterprise overlays, raw Odoo source, customer addons and training caches are not redistributed.

## Validation and limits

Windows: 522 application tests passed, plus compiled-payload regressions and isolated installer install/startup/removal. The acceptance installation preserved the existing user installation.

Ubuntu: 521 application tests passed, one private-bundle test skipped in the sanitized Community-only source snapshot, zero failures. Debian install, offscreen and X11 startup, compiled-payload regressions and removal passed.

The public Community runtime passed source-free migration smoke tests with original input preservation; the expected removed-model blocker was also verified. Owner training regressions: 373 passed. Detailed source commits, fingerprints, metrics, installer checks and SHA256 values are recorded in the platform manifests.

Static validation and canonical source knowledge do not prove an actual database's effective views or business compatibility. The customer Odoo install/workflow corpus was NOT_RUN. Test the migrated addon in the target Odoo environment before production. View retrieval metrics use retained-field identity proxies; they do not establish replacement precision for removed fields. The five-group 18-to-19 method holdout is small and does not establish universal rename coverage.

## Checksums and details

- [SHA256 checksums](SHA256SUMS-v1.0.7.txt)
- [Windows release notes](RELEASE_NOTES_v1.0.7.md) and [manifest](release-manifest-v1.0.7-windows.json)
- [Ubuntu release notes](RELEASE_NOTES_v1.0.7_UBUNTU.md) and [manifest](release-manifest-v1.0.7-ubuntu.json)

## Feedback

Use Issues for bug reports. Do not post credentials, customer data, proprietary source, Enterprise files or private logs publicly. The Windows installer may be unsigned and Microsoft SmartScreen may display a warning.

This repository distributes public installers and documentation. The application source repository is private.
