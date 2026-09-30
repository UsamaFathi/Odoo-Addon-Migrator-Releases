# Odoo Addon Migrator v1.0.3

Maintenance release for Windows and Ubuntu.

## Fixes

- Fixes Odoo 18→19 migrations that still reference `res.users.groups_id`; Odoo 19 defines this field as `group_ids`.
- Applies the rename only to parser-confirmed `res.users` records and `res.users` view architectures.
- Preserves unrelated models that may legitimately use a field named `groups_id`.
- Retains the Odoo 19 `res.groups.category_id` correction from v1.0.2.
- Includes Community and authorized Enterprise-derived migration knowledge in both desktop packages.

## Downloads

- Windows: `OdooAddonMigrator_Setup.exe`
- Ubuntu x86_64: `OdooAddonMigrator_1.0.3_amd64.deb`

The original addon directory remains unchanged. Static validation is not proof of runtime compatibility; install and test migrated addons on Odoo 19 before production use.

Independent migration utility. Not affiliated with Odoo S.A.
