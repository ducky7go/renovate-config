# renovate-config

Shared Renovate preset for the ducky7go org. The repo contains only `LICENSE` and `default.json`.

`default.json` (verified content) has the `$schema` `https://docs.renovatebot.com/renovate-schema.json` and `"extends": ["config:recommended"]`, i.e. it currently adds nothing beyond Renovate's recommended preset.

How it is consumed: a Renovate preset in a repo named `renovate-config` with `default.json` is referenced from other repos as `local>ducky7go/renovate-config` or `github>ducky7go/renovate-config` in their `renovate.json` `extends`. This is standard Renovate behaviour; no sibling checkout I inspected (SuperDucky, SuperDucky.Connector, SuperDucky.docs, DML) contains a Renovate config that references it yet.

Notes for editing:
- Keep the file valid JSON and Renovate-schema compliant; there is no CI or test in this repo.
- Changes affect every repo that extends this preset.
