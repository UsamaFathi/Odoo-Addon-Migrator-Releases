# Odoo Addon Migrator v1.0.2

Maintenance release for Windows and Ubuntu.

## Fixes

- Fixes Odoo 18→19 migrations that define `category_id` on `res.groups`, which Odoo 19 rejects with `ValueError: Invalid field 'category_id' in 'res.groups'`.
- Removes only the obsolete `category_id` field directly under `res.groups` XML records.
- Preserves `res.groups.privilege.category_id`, unrelated models, comments, and surrounding XML.
- Ensures the deterministic correction runs with the bundled Community + authorized Enterprise-derived Migration Brain, without requiring users to retrain or select a Brain.
- Retains the v1.0.1 fix for Odoo 16 `attrs` expressions containing list literals.

## Downloads

- Windows: `OdooAddonMigrator_Setup.exe`
- Ubuntu x86_64: `OdooAddonMigrator_1.0.2_amd64.deb`

The original addon directory remains unchanged. Static validation is not proof of runtime compatibility; install and test migrated addons on Odoo 19 before production use.

Independent migration utility. Not affiliated with Odoo S.A.
