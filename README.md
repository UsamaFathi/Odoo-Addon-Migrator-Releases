# Odoo Addon Migrator — Releases

Public desktop releases for **Odoo Addon Migrator**.

Odoo Addon Migrator helps developers migrate custom Odoo addons across supported versions from **Odoo 14 through Odoo 19** while keeping the original addon folder unchanged.

Every production desktop package published here includes both **Community migration knowledge** and **authorized Enterprise-derived migration knowledge**. End users select only their custom addons and migration versions; no Odoo source checkout, Enterprise source folder, training step, or runtime source indexing is required.

The packaged migration knowledge contains derived compatibility data only and does not contain Odoo Community or Enterprise source files.

## Downloads

Each stable version is published as **two separate GitHub Releases** so users can immediately choose the correct operating system.

### Windows release

Release tag format:

`v<version>-windows`

For v1.0.0:

`v1.0.0-windows`

Assets:

- `OdooAddonMigrator_Setup.exe` — recommended Windows installer.
- `OdooAddonMigrator-Windows.zip` — portable Windows build.
- `SHA256SUMS-Windows.txt` — checksums for the Windows packages.

### Ubuntu x86_64 release

Release tag format:

`v<version>-ubuntu`

For v1.0.0:

`v1.0.0-ubuntu`

Assets:

- `OdooAddonMigrator_1.0.0_amd64.deb` — recommended Ubuntu package.
- `OdooAddonMigrator-Ubuntu-x86_64.tar.gz` — portable Ubuntu build.
- `SHA256SUMS-Ubuntu.txt` — checksums for the Ubuntu packages.

Install the Debian package with:

```bash
sudo apt install ./OdooAddonMigrator_1.0.0_amd64.deb
```

Portable Ubuntu usage:

```bash
tar -xzf OdooAddonMigrator-Ubuntu-x86_64.tar.gz
cd OdooAddonMigrator
./OdooAddonMigrator
```

## What is bundled

Production releases include:

- Community migration knowledge for Odoo 14 through Odoo 19.
- Authorized Enterprise-derived migration knowledge for Odoo 14 through Odoo 19.
- The desktop migration engine and static validation workflow.

The production build process verifies that both migration-knowledge components are present before release artifacts are accepted.

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

The Windows installer may be unsigned, so Microsoft SmartScreen can display a warning.

## Checksums

Every stable platform release includes its own SHA-256 checksum file so downloaded packages can be verified before installation.

## Project note

This repository contains public release files and feedback resources only. Application development is maintained separately.

Odoo Addon Migrator is an independent migration utility and is not affiliated with Odoo S.A.
