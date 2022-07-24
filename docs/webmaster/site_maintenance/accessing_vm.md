If you need to access the VM that runs our site, you must connect using SSH.
Instructions for using SSH can be found [here][ssh-how-to].

You can connect via:

```terminal
ssh root@{{ site.base_url }}
```

Note: SSH connections can be refused if the VM is under high load. Because we
are using a memory constrained system, it's possible that SSH connections may
time out immediately after rebooting the VM. In this case, wait a few minutes
and try again. (But check that you can still access {{ site.base_url }} during this
time).

[ssh-how-to]: https://www.digitalocean.com/community/tutorials/how-to-use-ssh-to-connect-to-a-remote-server
