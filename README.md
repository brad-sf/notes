# notes.txt

## Ubuntu (14)

#### Create user
1. `adduser brad`
2. `gpasswd -a brad sudo`
3. `sudo usermod brad -aG www-data`

#### chmod file permissions correctly
- `sudo find /var/www -type d -print -exec chmod 775 {} \;`
- `sudo find /var/www -type f -print -exec chmod 644 {} \;`

## Unload
`sudo chown -R yourname:yourgroup *`


## SSH
`.ssh/config`
```
Host bradleyflood
Hostname bradleyflood.com
User brad
```

### Authorized keys
`chmod 700 ~/.ssh`
`chmod 600 ~/.authorized_keys`

## Upload files from local to remote via SSH
`scp /path/to/image.jpg username@bradleyflood.com:/var/www/bradleyflood.com/html/img/_private`


## Terminal

#### Find string in source code
- `curl -v --silent http://www.bradleyflood.com/ 2>&1 | grep 'crazyegg'`

### Curl with headers
- curl https://example.com/ -k -v

### Symlinks
- `ln -s /path/to/source/file /path/and/name/of/symlink`
- Eg `ls -s ~/www/dev/project /MyProjectShortcut`



## Git

Enable debug: `export GIT_TRACE=true`
