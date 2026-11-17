# Official Beta 1 catalog preparation — NOT INSTALLABLE / NOT PUBLISHED

This plan copies `Eion21/daimei@72ecd6dadb15a80c56de1d51e56fda2101a6cd37:distribution/official/s39/catalog-plan.json` exactly. All three `artifact` values are null; this is intentionally not a schema-2 installable catalog. No final signed artifact hash, size or URL has been invented.

Source export: `Daimei-Extensions/extensions-source@4fe7e9835e5cac98e458290c320177175de451ed`,95 byte-identical parent files; local commits only. Packages/source IDs/API contracts are unchanged. Matcha/Sky declare1.1; Jabra declares1.3, supported by the Beta1 host.

The chosen transport is strict HTTPS without redirects. After separate human authorization and signing, commit final extension APKs to a dedicated immutable path, capture that full40-character repository commit, verify exact hosted bytes and signer pins, and use commit-pinned `raw.githubusercontent.com/Daimei-Extensions/extensions-repo/...` artifact URLs. Do not use redirecting GitHub Release asset URLs or change origin allowlists. A stable catalog may later point to those immutable APKs; keep QA channels unchanged.

Use the exact parent source `tools/novel-distribution/prepare-official-catalog.py` following `docs/beta1-official-catalog.md` only on genuinely signed APKs. Canonical arguments must have no trailing newline; keep this plan repository fixed; choose a fresh non-symlink output on a hard-link-capable filesystem without a competing creator. The finalizer refuses unsigned APKs, mismatched official metadata/certificates, redirects and overwrites. Format-only fake-SDK tests are not real cryptographic verification.

Future signing must be explicitly authorized and use the user's private terminal. Verify both public pins, actual signed manifests/signers/source IDs and served SHA-256/size, then decode with the real host codec before separately authorizing publication. Never copy stores/passwords or development-signed local-candidate APKs into this channel. Nothing here changes existing QA, S38 or fixture evidence.

The old `LOCAL-CANDIDATE.md` and local development APKs remain historical preparation data, not Beta1 artifacts. This document supersedes their unresolved hosting/signing decision text for the new official plan only; it does not reinterpret historical runtime results. No push, tag, Release, signing or device operation was performed.
