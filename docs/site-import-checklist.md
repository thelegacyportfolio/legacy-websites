# Live Site Import Checklist

Use this checklist when bringing a production website under source control.

## Before importing

1. Create a host-level backup of website files and databases.
2. Inventory DNS, email records, cron jobs, redirects, PHP versions, and extensions.
3. Download files into a temporary working directory outside this repository.
4. Scan the download for secrets and customer or form-submission data.

## GuardianLock

Import deployable HTML, CSS, JavaScript, PHP, images, icons, manifests, and required server configuration into `sites/guardianlock.org/`.

Keep production videos on the host or CDN unless Git LFS is deliberately enabled. Exclude logs, support submissions, caches, backups, and secrets.

## The Legacy Portfolio

The live WordPress database and uploads require independent scheduled backups. Git should contain custom themes, custom plugins, safe configuration templates, and deployment documentation—not WordPress core, the database, or `wp-config.php`.

## Before committing

1. Review `git status` and every staged file.
2. Search for passwords, tokens, email credentials, private keys, and database connection strings.
3. Confirm no customer or form-submission data is present.
4. Test the site from the imported source.
