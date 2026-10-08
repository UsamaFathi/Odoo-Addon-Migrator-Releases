# Odoo Addon Migrator v1.0.5 - Windows

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
fingerprint are unchanged. Download fresh files, reinstall and rerun migration
into a new output folder. Inherited XPath review findings still need resolution.

Rebuilt v1.0.5 fixes the missing `sources/indexer.py` error when selecting a
custom addons folder. Frozen builds identify the indexer from bundled bytecode
and do not require loose application source files. The trained Brain is unchanged.

View Intelligence adds structural migration analysis for inherited Odoo views
across the supported 14 -> 15 -> 16 -> 17 -> 18 -> 19 path.

- Detects moved fields, visibility/widget/role changes, sibling and parent
  changes, repeated field occurrences and inheritance-operation risks.
- Reports missing, changed, risky and complex XPath anchors with source-free
  evidence and review-only candidate suggestions.
- Distinguishes STATICALLY_SUPPORTED canonical anchors from actual effective
  database compatibility. No speculative display_name replacement is applied.
- Includes the newly trained schema-v5 Community Brain with 17,319 view
  profiles and 84,699 field-anchor transitions.
- Keeps normal migration source-free and writes to a separate output directory.

The public installer bundles Community knowledge only. Enterprise overlays are
separate local-authorized artifacts and are not included in this release.

The trained Community API decision holdout measured zero false automatic fixes
across 7,177 decisions, with 65.59% coverage. The 18->19 view retrieval proxy
measured 99.89% precision with 77.32% coverage; this is retained-anchor retrieval,
not established semantic replacement accuracy. View candidates remain review-only.

Static validation is not runtime compatibility proof. Test migrated addons in
the target Odoo environment and inspect its effective inherited views.

Windows assets: installer, portable ZIP, SHA-256 checksums and release manifest.
Ubuntu uses a separate platform build and release tag.

Validation for this rebuild: 314 tests passed (one existing deprecation warning).
The portable executable and an isolated installation of the identical payload
passed the actual folder-selection/scan smoke without loose indexer source.
The existing user installation was left unchanged.
