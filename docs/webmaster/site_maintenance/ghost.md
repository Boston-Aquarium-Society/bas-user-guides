!!! warning "Backup Required"

    Before proceeding, make sure that the
    [site is backed up](/webmaster/site_maintenance/backup/).

You will need to SSH into our VM to perform the following maintenance. If you
do not know how to do so, read the
[accessing the VM](/webmaster/site_maintenance/accessing_vm) page first.

Make sure that NPM is up to date:

```terminal
npm install -g npm
```

Before proceeding, make sure to switch over to the Ghost manager account, and
move to our main Ghost directory (commands should not be run as root):

```terminal
sudo -i -u ghost-mgr
cd /var/www/ghost
```

Then, follow the [Ghost upgrade docs][ghost-upgrade-docs]. Because we operate in
a low memory environment, it's possible that Ghost might show an error saying
that it can not be upgraded due to insufficient memory. To address this, reboot
the VM via

```terminal
sudo reboot
```

and then re-SSH into the VM.

!!! info

    This will cause the VM to power cycle, which will take the site offline
    for a few seconds.

[ghost-upgrade-docs]: https://ghost.org/docs/update/
