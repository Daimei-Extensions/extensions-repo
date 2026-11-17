# extensions-repo
Official extension repository for Daimei

## Official Beta1 publication preparation — not live

Only genuinely signed/verified extension APKs may be published at `distribution/official/s39/beta1/{matchanovels-v1.0.2,skynovels-v1.0.2,jabrascan-v1.0.3}.apk`. They are not present yet. Sequence: publish extension source; commit/publish the three actual APKs; record the real full artifact commit and verify exact RawHTTPS served bytes; then generate/publish `official/s39/catalog.json` in a later commit with schema2 and commit-pinned raw.githubusercontent.com artifact URLs. No artifact SHA, size or future commit is invented. `official/s39/catalog-plan.json` remains noninstallable with null artifacts.

Planned stable URL (NOT live/verified yet): `https://raw.githubusercontent.com/Daimei-Extensions/extensions-repo/main/official/s39/catalog.json`. After publication: in Daimei Extensions overflow, choose Novel distribution (S39), paste that URL into the HTTPS schema2 field, add/query and review origin consent. The S38 read-only preview is not a repository subscription, and manga index/deep-link instructions do not apply. Download integrity, Android confirmation and explicit execution trust remain separate. Matcha/Sky use API1.1; JabraAPI1.3 is supported by the actual Beta1 host. App updates belong to https://github.com/Eion21/daimei/releases, not this channel.

No private keys/backups/passwords/credentials, debug/QA binaries, generic redirects or insecure CI signing. QA branches/history and S38 fixtures remain unchanged. See official/s39/PREPARATION.md for publisher constraints. No push, tag, Release or catalog publication is authorized by this documentation.
