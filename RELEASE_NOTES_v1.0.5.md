# Odoo Addon Migrator v1.0.5 - Windows

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
Ubuntu v1.0.5 is not published from this Windows build; its existing release
remains unchanged.

Validation: 274 tests passed with one existing deprecation warning; the owner's
training regression corpus passed 103 tests. Portable and installed GUI smoke
tests, silent installation and uninstallation passed. A source-free Community
15->19 migration smoke preserved its input and produced review findings.

The installer is unsigned. Independent migration utility; not affiliated with Odoo S.A.
