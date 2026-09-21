# wm-build-scratch

Temporary build runner. **No source code lives here** — the build clones it at
job time onto an ephemeral GitHub-hosted runner.

Exists only because public repos get unmetered GitHub Actions minutes and the
Microsoft Store (MSIX) package must be built on Windows.

Delete this repo once the MSIX is downloaded, and revoke the `SOURCE_PAT`
separately — deleting the repo does not revoke the token.
