# Odoo Addon Migrator v1.0.6 - Windows

This release adds guarded Python window-action tree/list conversion, broader
model-proven method-reference handling and newly trained Community migration
knowledge for Odoo 14 -> 15 -> 16 -> 17 -> 18 -> 19.

- Converts literal Python window-action `view_mode` and explicit `views` types
  from `tree` to `list` at the 17->18 step, including multi-hop migrations.
- Applies accepted method mappings to model overrides, self/cls/super uses,
  direct literal env-model calls and model-bound public XML object buttons.
- Leaves aliases, dynamic references, private RPC targets, signature/behavior
  changes and conflicting custom overrides for review.
- Preserves existing settings-layout, search-view, attrs and addon-identity fixes.
- Retains source-free View Intelligence and writes a separate output copy.
- Cleans stale app-owned package metadata during Windows upgrades so the new
  application version is reported correctly.

New Community Brain: schema 5; 210,564 training examples, 17,319 view profiles,
84,699 anchor transitions. Training regressions: 220 passed. Application tests
and packaged installation acceptance results are recorded in the release manifest.

Python rename validation is conservative and small: 7 accepted decisions from
29 trusted held-out groups, zero observed false suggestions, 24.14% coverage.
For 18->19: 1 accepted decision from 5 groups, 20% coverage. Git-history labels
were not enabled in this run. Thresholds were calibrated on this holdout; these
results are not independent business-runtime certification or support for all
method changes. Canonical source compatibility does not prove effective DB views.

The installer includes Community knowledge only. Enterprise overlays remain
local-authorized artifacts and are not distributed. No Odoo source checkout or
Python installation is required for normal desktop use.

Download `OdooAddonMigrator_Setup.exe`, close the app and install it. Rerun legacy
addons from their actual original Odoo version into a fresh output directory.
Review findings and test installation/business actions in target Odoo. Actual
Odoo install-corpus validation was NOT_RUN during training.

Installer-only release: no portable ZIP. Independent utility, not affiliated
with Odoo S.A. Existing v1.0.5 releases are preserved.

Validated release: 363 application tests passed on this platform; installer startup/removal and packaged Brain integrity passed.

SHA256 (`OdooAddonMigrator_Setup.exe`): `2eb347062c214c76d02da7799af6fb97e36e6edb35ee95f93392ff01c805392d`
