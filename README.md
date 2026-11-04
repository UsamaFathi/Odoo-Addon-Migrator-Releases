# Odoo Addon Migrator

Desktop migration assistant for custom Odoo addons, supporting forward upgrades along Odoo 14 -> 15 -> 16 -> 17 -> 18 -> 19.

## Download v1.0.8

| Platform | Installer | Tested environment |
|---|---|---|
| Windows x86_64 | [Download Windows installer](https://github.com/UsamaFathi/Odoo-Addon-Migrator-Releases/releases/download/v1.0.8-windows/OdooAddonMigrator_Setup.exe) | Windows, Python 3.12 bundled |
| Ubuntu x86_64 | [Download Debian installer](https://github.com/UsamaFathi/Odoo-Addon-Migrator-Releases/releases/download/v1.0.8-ubuntu/OdooAddonMigrator_1.0.8_amd64.deb) | Ubuntu 22.04.5 LTS |

Each release has one installer asset. No portable ZIP or tarball is published. Existing 1.0.7 and 1.0.6 releases remain available in [release history](https://github.com/UsamaFathi/Odoo-Addon-Migrator-Releases/releases).

## Changes in 1.0.8

- Newly trained, source-free schema-7 Community Brain with Python, XML, JavaScript and security compatibility facts.
- Import/export, model/decorator, XML data-tag/model-field, JavaScript export and downstream dependency checks.
- 23 additional guarded runtime-failure families, retaining the prior 85-case review catalog and contextual mappings.
- Correct target manifest versions, including duplicate keys and target-specific grammar.
- Existing view/XPath intelligence, Python tree/list actions, settings, column visibility, chatter and folder-handling safeguards retained.

Report cases remain contextual review knowledge. File inventory does not imply complete semantic migration of every file type. The tool preserves the original addon tree and writes a separate output with a report and diff.

## Install and use

Windows: run the setup executable, launch the application, select the original addons folder and the actual source/target versions, then migrate into a separate destination. Keep the complete installed application directory intact.

Ubuntu:

```bash
sudo apt install ./OdooAddonMigrator_1.0.8_amd64.deb
odoo-addon-migrator
```

End users do not need Python, official Odoo sources, training setup or CUDA. Public installers contain only Community-derived facts/model parameters. Enterprise overlays, raw Odoo source, customer addons and training caches are not redistributed.

## Validation and limits

Windows and Ubuntu: **586 application tests passed on each platform**, zero failures or skips. Compiled-payload regressions and installer install/startup/removal passed; Windows acceptance preserved the existing user installation. Ubuntu startup passed both offscreen and X11 checks.

The Community-only runtime passed source-free migration smoke tests with original input preservation and an expected removed-model blocker. Owner training regressions: **443 passed**. Schema 7 contains 210,564 examples, 17,319 view transitions and 84,699 anchor transitions. Source commits, fingerprints, measured metrics and installer SHA256 values are in the platform manifests. Full anonymous downloads of both installers matched the validated local SHA256 values.

Static validation and canonical source knowledge do not prove an actual database's effective views or business compatibility. The customer Odoo install/workflow corpus was NOT_RUN. Test the migrated addon in the target Odoo environment before production. View retrieval metrics use retained-field identity proxies; they do not establish replacement precision for removed fields. The five-group 18-to-19 method holdout is small and does not establish universal rename coverage.

## Checksums and details

- [SHA256 checksums](SHA256SUMS-v1.0.8.txt)
- [Windows release notes](RELEASE_NOTES_v1.0.8.md) and [manifest](release-manifest-v1.0.8-windows.json)
- [Ubuntu release notes](RELEASE_NOTES_v1.0.8_UBUNTU.md) and [manifest](release-manifest-v1.0.8-ubuntu.json)

## Feedback

Use Issues for bug reports. Do not post credentials, customer data, proprietary source, Enterprise files or private logs publicly. The Windows installer may be unsigned and Microsoft SmartScreen may display a warning.

This repository distributes public installers and documentation. The application source repository is private.
