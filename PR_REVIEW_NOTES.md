# Obsidian Releases PR Review Notes

This document captures the local checks performed for pull request [obsidianmd/obsidian-releases#8037](https://github.com/obsidianmd/obsidian-releases/pull/8037) and the items to monitor after submission.

## Local validation summary
- Manifest: `manifest.json` declares `id: "autotitle"`, `version: "1.0.0"`, and `minAppVersion: "0.15.0"`, matching the community entry.
- Release assets: GitHub release `1.0.0` contains `main.js`, `manifest.json`, `styles.css`.
- Documentation: `README.md` includes install, configuration, and usage guidance.
- License: `LICENSE` file present.

## GitHub follow-up checklist
- Confirm the release tag in `zaharenok/obsidian-autotitle` remains **1.0.0** so validator sees matching tag and manifest version.
- Ensure the PR body uses the community plugin template with all checkboxes marked.
- Wait for automation (`plugin-ci`) to complete successfully; investigate any failures (manifest mismatch, missing assets, formatting).
- Review bot comments for any requested metadata changes or clarifications.
- Monitor for human reviewer feedback; update release/README if requested.

## GitHub status
- PR link: https://github.com/obsidianmd/obsidian-releases/pull/8037
- Current checks: to be verified in GitHub UI (look for green `plugin-ci`, no merge conflicts).
- Mergeability: ensure “This branch has no conflicts” and all required checks pass.

## If validation fails
If the validator or reviewers request changes, update the plugin repository (fix manifest, refresh release assets, or bump version), publish a new release tag, and re-run PR checks.
