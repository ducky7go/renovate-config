# renovate-config

Shared Renovate preset for the ducky7go org. The repo holds `default.json` and `LICENSE`.

- `default.json` sets `$schema` to `https://docs.renovatebot.com/renovate-schema.json` and `"extends": ["config:recommended"]`. It adds nothing beyond Renovate's recommended preset.
- Consumers reference it from `renovate.json` as `github>ducky7go/renovate-config` (or `local>ducky7go/renovate-config`). For example, `Ducky.Samples/renovate.json` uses the `github>` form.

## Notes for editing

- Keep `default.json` valid JSON and Renovate-schema compliant. The repo has no CI or tests, so check the file by hand.
- Every repo that extends this preset is affected by a change here.
