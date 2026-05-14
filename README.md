# papiflyfx-build-parent

Extracted from the PapiflyFX Docking monorepo.

## Modules


## Build

Use the split-local Maven repository so cross-repo snapshots resolve from the extraction workspace:

```bash
./mvnw -Dmaven.repo.local=$HOME/github/papiflyfx/.m2-split -Dtestfx.headless=true clean verify
```

Lead agent: `@ops-engineer`.

## Notes

- This parent has no child modules. The `it/smoke-consumer` POM inherits from it for a minimal parent-resolution check.
