# Legacy Portfolio Websites

Source-controlled website assets for Legacy Portfolio properties.

## Sites

- `sites/guardianlock.org/` — GuardianLock public website source and deployable assets.
- `sites/thelegacyportfolio.org/` — custom WordPress themes, plugins, and deployment configuration for The Legacy Portfolio.

## Repository boundaries

This repository stores maintainable source code and normal web assets. It does not replace production backups.

Never commit:

- passwords, API keys, access tokens, or private certificates;
- WordPress database dumps or `wp-config.php`;
- form submissions, customer data, logs, caches, or generated backups;
- dependency directories or server-generated files;
- large production videos unless they are intentionally managed with Git LFS.

See [`docs/site-import-checklist.md`](docs/site-import-checklist.md) before importing files from a live host.
