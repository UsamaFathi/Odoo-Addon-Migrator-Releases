# Odoo Addon Migrator v1.0.5 - Ubuntu x86_64

The latest rebuild adds an explicit technical addon-name review when a version-suffixed
folder still refers to locally declared XML IDs under its original namespace.
Confirm the intended name before migration. Only the output copy's folder name
changes; XML IDs, Python references and permissions are not speculatively rewritten.
Single-addon selections now produce an output container containing the addon folder.
Ambiguous ownership remains for review. The original addon tree is unchanged.

Manifests identify `module-identity-fix`, application commit `450ec4d`, and
314 passing tests on each platform. Existing settings, search-view, attrs and
folder-selection fixes are retained. The schema-v5 Brain and Enterprise overlay
binding are unchanged; no retraining is required. Download fresh files, reinstall
and rerun migration into a new output folder.

A fresh migrated addon with an explicitly selected original technical name
installed successfully in isolated Odoo 19, including resolution of its manager
group XML ID. Customer database upgrades and business workflows were not tested.

The earlier settings rebuild fixes canonical legacy `res.config.settings` app insertions:
complete named app blocks inserted inside the removed `div.settings` move to
named `app` nodes inside `//form`. Inner fields, labels, help, modifiers and
layout are preserved. Partial/ambiguous inheritance operations remain for review.
Literal settings-form actions also migrate the removed Odoo 19 `inline` target
to `current`. Both rules work with existing trained Brains; no retraining is
required. Those settings rules were introduced in code commit `e86741b`.

The earlier settings-only install check stopped later on a custom namespace
mismatch. The explicitly selected-name install check described above supersedes
that result; it does not validate every customer database composition.

The latest v1.0.5 rebuild fixes Odoo 19 search-view validation by removing
legacy `expand` and `string` attributes from search-view groups. Legacy
boolean `attrs` modifiers and quoted values containing `>` are converted
correctly. No Brain retraining is required; schema 5 and the Community
fingerprint are unchanged. Download fresh files and rerun migration into a
new output folder. Inherited XPath review findings still need resolution.

Rebuilt v1.0.5 fixes the missing `sources/indexer.py` error when selecting a
custom addons folder. Frozen cache identity uses bundled bytecode; no loose
application source files are required. The trained Community Brain is unchanged.

View Intelligence analyzes inherited-view changes across Odoo
14 -> 15 -> 16 -> 17 -> 18 -> 19, including moved or hidden fields,
parent/sibling changes, repeated occurrences and fragile XPath anchors.
Candidates remain suggestions for review; ambiguous XML is not rewritten.

Includes the same schema-v5 Community Brain as Windows v1.0.5:
17,319 view profiles and 84,699 anchor transitions. Enterprise overlays are
separate local-authorized artifacts and are not included.

Validation: 314 tests passed in Ubuntu 22.04.5. The portable application,
Debian installation in an isolated cached Ubuntu VM, installed offscreen and
X11 GUI smoke tests, and package removal passed. Source-free Community
15->19 migration preserved its input and did not index Odoo source.

Requirements: Ubuntu 22.04 x86_64; CPU support for SSSE3, SSE4.1, SSE4.2 and
POPCNT (Qt 6.11). Validated in a 4 GB VM; 8 GB RAM is recommended. A 2 GB VM
was insufficient. During initial v1.0.5 validation, measured startup peak was approximately 2.14 GiB resident
memory, and startup took about 38 seconds while loading/verifying the Brain.

Assets:

- `OdooAddonMigrator_1.0.5_amd64.deb`
- `OdooAddonMigrator-Ubuntu-x86_64.tar.gz`
- `SHA256SUMS-Ubuntu.txt`
- `release-manifest-ubuntu.json`

Install:

```bash
sudo apt install ./OdooAddonMigrator_1.0.5_amd64.deb
odoo-addon-migrator
```

Static compatibility is not effective database-view or runtime Odoo proof.
Test migrated addons in the target Odoo environment. The original addon tree
remains unchanged. No Odoo 20 or downgrade support.

Independent migration utility; not affiliated with Odoo S.A.
