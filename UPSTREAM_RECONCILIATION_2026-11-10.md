# Original-source reconciliation — 2026-11-10

**Review checklist, not completed upstream merge.**

- Original: cavinpabua/fv-launcher @ 47958330199ea21d6e4e3a6b0b84fea58ac309ce
- Upstream snapshot: upstream-sync/2026-11-10
- Fork backup: backup/pre-upstream-sync-2026-11-10
- Git histories unrelated. Direct PR rejected with HTTP 422.
- 7 conflicts: .github/workflows/build.yml, .gitignore, README.md, main.js, package-lock.json, package.json, preload.js.
- Preserve Electron repair/download scripts and tests. Source adds prebuilt PepperFlash binaries, which must not be restored without review.

## Completion gates
1. Build a true merge from an isolated fork branch, allowing unrelated histories and resolving each overlapping file deliberately.
2. Preserve fork-specific work, and never reset or force-push the default branch.
3. Run build, tests, and security/dependency review before merging code.
4. Retain both pinned snapshots until validation.
