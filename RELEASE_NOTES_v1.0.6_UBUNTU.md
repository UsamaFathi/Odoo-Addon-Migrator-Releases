# Odoo Addon Migrator v1.0.6 Fixed - Ubuntu x86_64

This **v1.0.6 Fixed** build corrects addon-folder naming review and Windows
staging permissions. The application/package version remains 1.0.6.

- Excludes Git metadata from migrated copies, avoiding repository locks during
  the final output-directory move.
- Makes copied read-only files writable without changing original files.
- Requests an explicit valid technical name for addon folders containing dots,
  spaces or hyphens; no guessed name or automatic reference rewrite.
- Retains full error tracebacks and identifies the last reported operation stage.
- Keeps naming validation readable under Windows dark system defaults.

No retraining is required. The Community Brain is unchanged, and Enterprise
knowledge remains local only. Both releases contain one installer asset, with
no portable ZIP/tarball. Close the tool and reinstall the fixed installer even
if your installed version already says 1.0.6.

Includes the same newly trained schema-v5 Community Brain and Python/View
Intelligence changes as Windows v1.0.6. Python window-action tree/list conversion
belongs to 17->18 and runs in composed upgrades. Model-proven method references
are supported; ambiguous references, private RPC methods and behavior changes
remain for review. Existing settings, search-view and addon-identity fixes remain.

Community knowledge: 210,564 training examples, 17,319 view profiles and 84,699
anchor transitions. Python rename calibration holdout: 7 accepted decisions from
29 trusted groups, zero observed false suggestions; 18->19 accepted 1 of 5.
These small source-evidence samples are not comprehensive method support or
runtime compatibility proof. Actual Odoo install-corpus validation was NOT_RUN
during training. Package/test acceptance results are in the release manifest.

Community-only, source-free runtime. Enterprise overlays are not distributed.
Original addons remain unchanged; rerun from the actual original source version
into a fresh output directory and review/install-test the result.

Requirements: Ubuntu 22.04 x86_64 or compatible later environment; SSSE3, SSE4.1,
SSE4.2 and POPCNT CPU support for bundled Qt. 8 GB RAM recommended; earlier
acceptance required a 4 GB VM. A 2 GB VM was insufficient. Startup verifies and
loads the Brain and can take time. No Python/CUDA installation is required.

Installer-only release: `OdooAddonMigrator_1.0.6_amd64.deb`; no portable tarball.

```bash
sudo apt install ./OdooAddonMigrator_1.0.6_amd64.deb
odoo-addon-migrator
```

Independent utility, not affiliated with Odoo S.A. Earlier release notes remain in the public repository.

Validation: 369 application tests passed on this platform; installed startup/removal and frozen fix regressions passed.

SHA256 (`OdooAddonMigrator_1.0.6_amd64.deb`): `e77cd105c612cd8478fe0fe3eaf9ae995fcfa35de00da2cea415deb5ae05821c`
