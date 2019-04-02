# Wordpress

## Reconnaissance

#### Default Files

```
wp-login.php
wp-config.php
wp-register.php
```

#### Default Folders

```
/wp-content
/wp-content/plugins
/wp-content/themes
/wp-admin
```

#### Determine Version

> Search the source code for generator, and look for a line similar to this

```html
<meta name="generator" content="WordPress 4.9.7" />
```

#### Enumerating Users

**Possible URLs**

```
/author.php?id={id}
/author-{nicename}.php
/author-{id}.php
/author/{nicename}
```

**Check RSS feed**
http://domain.com/feed/

Look for the following

```xml
<dc:creator><![CDATA[Some Name]]></dc:creator>
```

## Tools

* [WPScan](https://wpscan.org/)

## Google Hacking

