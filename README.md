# Odoo Addon Migrator — Releases

Public desktop releases for **Odoo Addon Migrator**.

Odoo Addon Migrator helps developers migrate custom Odoo addons across supported versions from **Odoo 14 through Odoo 19** while keeping the original addon folder unchanged.

## Downloads

Open the **Releases** section of this repository and download the package for your operating system.

### Windows

**Recommended**
- `OdooAddonMigrator_Setup.exe` — Windows installer.

**Portable**
- `OdooAddonMigrator-Windows.zip` — extract and run `OdooAddonMigrator.exe`.

### Ubuntu x86_64

**Recommended**
- `OdooAddonMigrator_<version>_amd64.deb`

Install with:

```bash
sudo apt install ./OdooAddonMigrator_*_amd64.deb
```

**Portable**
- `OdooAddonMigrator-Ubuntu-x86_64.tar.gz`

Run with:

```bash
tar -xzf OdooAddonMigrator-Ubuntu-x86_64.tar.gz
cd OdooAddonMigrator
./OdooAddonMigrator
```

## Typical workflow

1. Select the custom addons folder.
2. Confirm or choose the source Odoo version.
3. Choose the target Odoo version.
4. Choose a separate output folder.
5. Start the migration.
6. Review the migration report and diff.
7. Install and test the migrated addons on the target Odoo environment.

The original custom addon folder is not modified by the migration workflow.

## Feedback and bug reports

We are actively collecting real migration experience to improve compatibility and usability.

Use the repository **Issues** section and choose:
- **Bug report** for crashes, installation problems, incorrect migrations, or validation problems.
- **Product feedback** to share migration results, manual fixes that were still required, and UI/workflow feedback.

Please do **not** post credentials, customer data, proprietary addon source code, private logs containing secrets, or other sensitive information in public issues.

## Validation and production use

Static migration and validation cannot guarantee production compatibility. Always install and test migrated addons on the target Odoo version before using them in production.

The Windows build may be unsigned, so Microsoft SmartScreen can display a warning.

## Checksums

Stable releases include `SHA256SUMS.txt` so downloaded files can be verified before installation.

## Project note

This repository contains public release files and feedback resources only. Application development is maintained separately.

Odoo Addon Migrator is an independent migration utility and is not affiliated with Odoo S.A.
