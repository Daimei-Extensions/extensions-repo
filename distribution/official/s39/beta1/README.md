# Official Beta1 signed extension artifacts

These three APKs are the exact human-signed official release bytes, verified with Android SDK; not QA, Debug or unsigned builds. Source APK commit: `72ecd6dadb15a80c56de1d51e56fda2101a6cd37`. Extension-source preparation head: `6968489a430fd4d09ed4d0148b777000e1fd0811` (source-content snapshot `4fe7e9835e5cac98e458290c320177175de451ed`).

Official singleton certificate SHA-256: `2782d342e313fe5cb3ca81996f084661a4eb21bbf11e139d8c3913edacf75408`.

| File | Signed bytes | Signed SHA-256 |
|---|---:|---|
| matchanovels-v1.0.2.apk | 213651 | `0479d428c7412c8b7c29f4fdc10aa0ef36b50ea526cafa1c319b246f829ba9b9` |
| skynovels-v1.0.2.apk | 33359 | `b63a8397e01d3ebb36bb71c7c530b38dfaec5f3d00b9caeb46512e3bcdd885b0` |
| jabrascan-v1.0.3.apk | 8483239 | `07bccd61a21231adf3dfd0afddfb66f0497aaf6dec6733e09a342beda597e51d` |

Use full-commit raw.githubusercontent.com URLs naming the commit that first contains these exact bytes. The schema2 catalog is committed separately afterward at `official/s39/catalog.json`; its stable main URL is not a publication claim until authorized push and direct served-byte verification. Do not rebuild, re-sign, realign or substitute CI artifacts. No .idsig, unsigned, QA APK, private key or password is part of this directory. Licenses and source attribution remain in the extension source repository. Runtime smoke test of the public app is separately pending.
