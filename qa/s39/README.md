# S39 experimental distribution QA — NOT an official release

This isolated branch hosts one pre-existing disposable extension APK and a `daimei-novel-distribution` schema2 catalog for a separately authorized Daimei S39 QA installation gate. It does not publish Daimei, MatchaNovels, SkyNovels or JabraScan releases. Do not install this fixture in a production reader or infer trust from its presence here.

## Exact fixture and declarations

- Package: `app.novel.extension.fixtures`, version1.0.0/code1, minSdk26, novel-api1.1.
- Sources: `fixture-extension` (synthetic offline sample) and `http-fixture-extension` (emulator-only10.0.2.2 HTTP fixture; do not fetch its content on a physical phone). An image uses the intentionally non-resolving fixture.invalid host.
- Existing Android Debug development/QA certificate, not a production or unique per-fixture key. No private key, keystore, password, device record or local configuration is included.
- `artifact-metadata.json` describes the original inspected bytes. `SHA256SUMS` covers the APK and catalog. No APK rebuild, host app rebuild or certificate change occurred for hosting.
- The original project's licenses and attribution remain applicable; this is not a dependency-license audit.

## Commit-pinned artifact

The catalog points to this exact artifact commit: `93c87fd3f615a84e5290cd8b512973fcc78a64db`.
Artifact URL: `https://raw.githubusercontent.com/Daimei-Extensions/extensions-repo/93c87fd3f615a84e5290cd8b512973fcc78a64db/qa/s39/novel-fixtures-extension-1.0.0-qa.apk`.

The catalog is `catalog.json` beside this README. Use a Raw URL with the full commit ID containing that catalog, not a mutable branch reference. Neither commit-address construction nor a local parser result asserts remote availability: direct anonymous HTTPS200, no redirects, bytes/size/hash and the unchanged S39 origin policy must be observed after the single authorized push. Never weaken the policy or retry a failed push automatically.

## Trust and Android boundary

Hashes and signer declarations from the same catalog are untrusted expectations, not independent authenticity, cryptographic preinstallation proof or execution authority. Keep repository enrollment, artifact-origin consent, normal Android confirmation and explicit scoped execution trust separate. No automatic trust/load, silent installation, public installer activation or Android test follows this publication.

Installation/rejection, reconciliation, execution gating, source recognition, restart and updates are NOT proved by hosting. They need a separate explicit human grant. This branch must not change main, qa-s38-readonly, historical fixtures, Actions or protection rules.
