# Korean translation validation

Catalog additions against `68e58a2eae462ba997a8ba5a1269e03a79b61136`: **4** entries. Existing Korean entries are unchanged. The provided translation data was checked against the current Rust sources; candidate keys with no matching production literal were excluded. No new translations were generated.

## Static checks

- Catalog structure, unique keys, original key preservation, named placeholders, trailing ellipses, and explicit shortcut tokens checked with Python 3.14.5.
- Existing catalog entries were compared with the baseline commit.
- New entries have source-location evidence in the local audit; dynamic labels use the existing translation paths.
- `git diff --check` passed.

## Checks not run

Cargo, rustc, and rustfmt are unavailable in this environment. Rust installation is awaiting user approval; no tools were installed. The following checks have **not** been run:

- `cargo test -p gridcraft-ui-egui`
- `cargo fmt --all --check`
- `cargo clippy -p gridcraft-ui-egui --all-targets -- -D warnings`
- `cargo xtask layers`, `cargo xtask assets`, `cargo xtask wasm`, and the full `cargo xtask ci` gate
- Native and web UI rendering, layout, runtime language switching, and font/glyph coverage

## Candidate filtering

- Excluded 21 supplied candidate keys without a matching production source literal.
- Excluded 553 supplied keys already proposed in open Korean translation PRs.

- https://github.com/storytold/gridcraft/pull/1426
