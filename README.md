# notes.txt

## Ubuntu 14

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

## Terminal

#### Find string in source code
- `curl -v --silent http://www.bradleyflood.com/ 2>&1 | grep 'crazyegg'`

### Curl with headers
- curl https://example.com/ -k -v
