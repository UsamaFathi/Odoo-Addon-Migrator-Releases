# Odoo Addon Migrator v1.0.4 for Windows

Maintenance release for the Windows desktop application.

## Fixes

- Adds source-backed Odoo 19 view-anchor knowledge to the bundled migration Brain.
- Detects genuinely missing inherited-view XPath field anchors as review-required findings.
- Avoids unsafe automatic replacement of valid Odoo 19 anchors such as `display_name`.
- Preserves the original addon directory and keeps migration output separate.
- Includes Community and authorized Enterprise-derived migration knowledge.

## Download

- Windows: `OdooAddonMigrator_Setup.exe`

Ubuntu v1.0.4 is not published yet. The latest available Ubuntu package remains v1.0.3.

Static validation is not proof of runtime compatibility; install and test migrated addons on the target Odoo version before production use.

Independent migration utility. Not affiliated with Odoo S.A.
