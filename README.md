# Odoo Addon Migrator — Releases

Public binary releases for **Odoo Addon Migrator**.

Odoo Addon Migrator is a desktop migration assistant for custom Odoo addons, supporting migration paths across **Odoo 14 → 19**.

## Downloads

Open the **Releases** section of this repository and choose the package for your operating system.

### Windows

**Recommended**
- `OdooAddonMigrator_Setup.exe` — Windows installer.

**Portable**
- `OdooAddonMigrator-Windows.zip` — extract and run `OdooAddonMigrator.exe`.

### Ubuntu x86_64

**Recommended**
- `OdooAddonMigrator_<version>_amd64.deb` — Ubuntu/Debian installer.

Install with:

```bash
sudo apt install ./OdooAddonMigrator_*_amd64.deb
```

Then open **Odoo Addon Migrator** from the applications menu.

**Portable**
- `OdooAddonMigrator-Ubuntu-x86_64.tar.gz`

Run with:

```bash
tar -xzf OdooAddonMigrator-Ubuntu-x86_64.tar.gz
cd OdooAddonMigrator
./OdooAddonMigrator
```

## Odoo source choices

For every required Odoo version, the application supports either:

- **Local Exact Source** — select an existing local Odoo source tree. It is read-only and is never modified.
- **Verified Snapshot** — use the pinned official Odoo Community source snapshot. If it is not cached, the application asks before downloading it.

Git is only required when downloading verified snapshots.

## Release status

Current builds are **release candidates**. Static validation does not guarantee runtime or production compatibility. Always install and test migrated addons on the target Odoo version before production use.

The Windows build is currently unsigned, so Microsoft SmartScreen may show a warning.

## Project note

This repository contains **binary release files only**. The application source repository is maintained separately.

Odoo Addon Migrator is an independent migration utility and is not affiliated with Odoo S.A.
