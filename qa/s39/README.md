# S39 experimental distribution QA — not a release

This directory contains one disposable test extension for a separately authorized Daimei S39 QA installation gate. Do not install it in a production reader or treat it as a trusted official source. MatchaNovels, SkyNovels, JabraScan and Daimei app APKs are not distributed here.

- Package: `app.novel.extension.fixtures`, version1.0.0/code1, minSdk26, novel-api1.1.
- Existing Android Debug development/QA signer; no production key, keystore or credentials are included. Its public certificate is not an execution grant.
- The APK is the pre-existing test artifact; no rebuild or new certificate was performed for hosting.
- Source IDs: `fixture-extension` and `http-fixture-extension`. The HTTP source targets an emulator-only10.0.2.2 fixture server; do not invoke its content requests on a physical phone. The self-contained source contains synthetic sample content and a non-resolving fixture.invalid image reference.
- The original project's licenses and attributions remain applicable. This metadata is not a dependency-license audit.

`artifact-metadata.json` and `SHA256SUMS` describe these exact bytes. A subsequent commit adds the existing schema2 catalog with an artifact URL pinned to this artifact commit. Before publication, that URL is a planned address, not a live endpoint.

Matching a hash from the same catalog proves only byte agreement, not independent authenticity. Repository enrollment, artifact-origin consent, normal Android installer confirmation and explicit execution trust remain separate. Public installation stays disabled; do not bypass any gate. No Samsung operation or automatic Android test follows hosting publication.
