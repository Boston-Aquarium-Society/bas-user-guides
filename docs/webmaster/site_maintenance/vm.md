!!! warning "Backup Required"

    Before proceeding, make sure that the
    [site is backed up](/webmaster/site_maintenance/backup/).

## Package Updates

Our VM is configured to automatically install security patches and other updates.
Therefore, it's unlikely that running these commands will result in any updates.

```terminal
sudo apt-get update
sudo apt-get upgrade -y
```

## Kernel upgrades

The VM's kernel should be updated from time to time. To do so, follow the
[instructions here][kernel-upgrades]. Note that kernel upgrades will require
powering down and restarting the VM, which will result in site downtime.

These steps should be performed during times of low traffic.

[kernel-upgrades]: https://docs.digitalocean.com/products/droplets/how-to/kernel/upgrade/
