# Odoo Addon Migrator v1.0.0

First stable public desktop release for Windows and Ubuntu x86_64.

## Supported migration range

Odoo 14 through Odoo 19 using adjacent migration steps for multi-version upgrades.

## Windows

- `OdooAddonMigrator_Setup.exe` — recommended installer.
- `OdooAddonMigrator-Windows.zip` — portable build.

## Ubuntu x86_64

- `OdooAddonMigrator_1.0.0_amd64.deb` — recommended Debian/Ubuntu package.
- `OdooAddonMigrator-Ubuntu-x86_64.tar.gz` — portable build.

## Highlights

- Local desktop workflow; the original custom addon folder is never modified.
- Separate migrated output directory.
- Automatic migration and static validation across supported Odoo versions.
- Bundled Community and authorized Enterprise-derived migration knowledge; no Odoo source checkout is required by end users.
- The bundled knowledge contains derived compatibility data only and does not contain Odoo Community or Enterprise source files.
- Python, XML, manifest, security, JavaScript, view, and compatibility transformations.
- Multi-hop migrations such as 16 → 18 and 16 → 19.
- Migration report and diff for review.
- Windows and Ubuntu desktop packages.
- SHA-256 checksums published with release files.

## Feedback

Please use the repository issue templates to report bugs and migration experience. Do not post credentials, customer data, or proprietary source code in public issues.

## Important

Static migration and validation cannot guarantee production compatibility. Always install and test the migrated addons on a target Odoo environment before production use.

Odoo Addon Migrator is an independent migration utility and is not affiliated with Odoo S.A.
