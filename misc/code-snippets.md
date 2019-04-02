# Code Snippets

**Wayback machine search alias for .bashrc / .bash_aliases**
```
waybackurls() {
  curl --silent "http://web.archive.org/cdx/search/cdx?url=$1*&output=text&fl=original&collapse=urlkey"
}
```

**Find open redirects from wayback machine**
```bash
$ waybackurls example.com | grep -iE '[?|&][url|uri|redir|dest|next].+=http.+[^&]'
```

**Download client side source code of modern SPA websites**
```
$ waybackurls example.com > waybackurls.txt
$ for url in `cat waybackurls.txt`; do wget $url; done
```
