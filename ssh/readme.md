# SSH

## Links
* Why root login should be disabled: https://unix.stackexchange.com/q/82626

## Configuration
Open SSH config file: `sudo vi /etc/ssh/sshd_config`
1. Disable root SSH login: `PermitRootLogin no`
2. Change SSH port: `Port 54553`
3. Disable password authentication: `PasswordAuthentication no`
4. Disable the use of empty passwords: `PermitEmptyPasswords no`
5. Disable X11Forwarding: `X11Forwarding no`
6. Restart SSH service: `sudo systemctl restart sshd`

Login to server using configured port:
```console
$ ssh -p 54553 leo@116.202.13.252
```