# Bizbox

This project was designed for x64 machines running Ubuntu Server 20.04 or 22.04. 

Before installling Bizbox or sandbox apps you need to follow these steps :

### Requirements

- [Sb](https://github.com/jeremiahg7/Sb/)

### Bizbox preinstall

This step will create the user account specified in accounts.yml (default=saltbox), add it to sudoers, update the kernel, edit GRUB configuration, install Rclone, and reboot the server if needed.

Edit accounts.yml file to specify user and password

```
cd /srv/git/bizbox
vi accounts.yml
```

```
sb install preinstall
```

If your server did not need to reboot you can run su username to switch user or reconnect to SSH as the newly created user. Everything after this point will assume you are running as the user entered in accounts.yml

### [Install sandbox apps](https://github.com/jeremiahg7/Sandbox/)
