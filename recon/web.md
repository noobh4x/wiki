# Web Reconnaissance

## Google Hacking

  * [Google Hacking](https://github.com/noobh4x/wiki/blob/master/recon/google-hacking.md)

## User Enumeration

**Verbose error messages on failed logins**

When attempting to log in, some sites will return verbose errors disclosing if the user was found in their system or not.

**Password recovery**

Using the password recovery will in many situations (in)directly tell if the username/email was found.

## Wayback Machine

> Replace example.com with any domain

`http://web.archive.org/cdx/search/cdx?url=example.com*&output=text&fl=original&collapse=urlkey`

To make things a bit easier, make an alias in `~/.bashrc` or `~/.bash_aliases`

```
waybackurls() {                                                                 
    curl --silent "http://web.archive.org/cdx/search/cdx?url=$1*&output=text&fl=original&collapse=urlkey"               
}
```

Usage:
```
$ waybackurls example.com
```

### Download Source Code
```
$ waybackurls example.com > domains.txt
$ for line in `cat domains.txt`; do wget $line; done
```
