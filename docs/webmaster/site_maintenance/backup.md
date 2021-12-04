You must always create a backup of the site before performing any maintance as
a safeguard against data loss.

There are two types of backups configured on our site:

1. VM level backups: Digital Ocean backs up the full site weekly, and each
   backup is stored for 4 weeks. More documentation about this can be found
   [here][do-backup-docs]. These backups can be used to perform a full system
   restore if the host running the site was damaged beyond repair.
1. Site-level backups: You can download a JSON file with all site content
   by navigating to the site [labs settings][labs-settings], then clicking the
   `Export` button.

**Do not proceed with any site maintenance before confirming that a backup exists.**

[do-backup-docs]: https://docs.digitalocean.com/products/images/backups/
[ghost-backup-docs]: https://ghost.org/help/the-importer/#exports-in-ghost
[labs-settings]: https://https://{{ site.url }}/ghost/settings/labs
