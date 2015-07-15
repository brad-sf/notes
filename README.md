# notes.txt

## Ubuntu 14

#### Create user
1. `adduser brad`
2. `gpasswd -a brad sudo`

#### chmod file permissions correctly
- `sudo find /var/www -type d -print -exec chmod 755 {} \;`
- `sudo find /var/www -type f -print -exec chmod 644 {} \;`
