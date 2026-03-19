# AGENTS.md

This repository is maintained by AI assistance (OpenClaw).

## Goal

- Support **Laravel 13+ only**
- Minimum PHP: **8.3**
- Keep a clean CI signal (tests + lint/format) before tagging a release

## Local workflow

```bash
composer install
composer check-style
```

## Release workflow

1. Ensure `composer.json` supports Laravel 13 / PHP 8.3.
2. Run code quality checks (Pint) and any test suite (if present).
3. Commit changes.
4. Wait for GitHub Actions to pass.
5. Tag & publish release using `gh release create`.

## Notes

- This package is a Laravel wrapper for `w7corp/easywechat`.
- If Laravel introduces contract signature changes, prefer updating the wrapper to match Laravel 13 APIs.
