# Odoo Addon Migrator v1.0.1

Maintenance release for Windows and Ubuntu x86_64.

## Fixed

- Fixed a migration crash when an Odoo 16 `attrs` domain contains a list literal, including expressions such as `('state', 'not in', ['done'])`.
- Unsupported modifier expressions remain unchanged and visible for review instead of aborting the complete migration.

## Included

- Odoo 14 through 19 migration support.
- Bundled Community and authorized Enterprise-derived migration knowledge; end users do not need Odoo source checkouts.
- Separate output migration that does not modify the original addon directory.
- Human-readable migration report, diff, and static validation result.

Static validation does not prove runtime compatibility. Install and test migrated addons on the target Odoo version before production use.

Odoo Addon Migrator is an independent migration utility and is not affiliated with Odoo S.A.
