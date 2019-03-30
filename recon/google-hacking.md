# Google Hacking

## Resources

**Knowledge**

  * [Refine web searches](https://support.google.com/websearch/answer/2466433?hl=en) (Google)
  * [Google Search Operators](https://moz.com/learn/seo/search-operators) (Mozilla)

**Databases**

  * [Google Hacking Database](http://exploit-db.com/ghdb) (exploit-db.com)

## Operators

### Basic Search Operators

| Operator | Description                     |
|----------|---------------------------------|
| @        | Search social media / usernames |
| #        | Search for hashtags             |
| $        | Search for prices in dollar     |
| €        | Search for prices in euro       |
| ..       | Search for number range         |
| -        | Exclude words                   |
| "..."    | Find exact match                |
| *        | Wildcard                        |
| OR       | Combine search                  |
| %%|%%    | Alias of OR                     |
| ()       | Group operators                 |
| in       | Convert between units           |

### Advanced Search Operators

| Operator    | Description                                         |
|-------------|-----------------------------------------------------|
| intitle:    | Search only in page titles. Use quotes with phrases |
| allintitle: | Same as multiple intitle:                           |
| inurl:      | Search for content in the URL                       |
| allinurl:   | Same as multiple inurl:                             |
| intext:     | Search in the document body content                 |
| allintext:  | Same as multiple intext:                            |
| filetype:   | Find specific filetypes                             |
| related:    | Find sites related to another site                  |
| site:       | Return results from a specific site                 |
| info:       | Get info about a site                               |
| cache:      | Cached version of a site                            |
| AROUND(x)   | Find pages where two phrases are around X words     |

### Unreliable / Deprecated Operators

| Operator     | Description                                                           |
|--------------|-----------------------------------------------------------------------|
| ~            | Includes synonyms, which also currently is default behavior           |
| +            | Exact match on single words/phrases. Deprecated after Google+ release |
| daterange:   | Find results in specific date range. Requires Julian dates            |
| link:        | Find pages linking to target domain                                   |
| inanchor:    | Find anchors with a specific text                                     |
| allinanchor: | Same as multiple inanchor:                                            |

## Dorks

### Passwords

  * [Credentials in public Trello boards #1](https://www.google.com/search?q=site:trello.com%20AND%20intext:username%20AND%20intext:password)
  * [Credentials in public Trello boards #2](https://google.com/search?q=inurl:https://trello\.com%20AND%20intext:@gmail\.com%20AND%20intext:password)

### Sensitive Files

  * [Apache status page](https://google.com/search?q=intitle:%22Apache%20Status%22%20intext:%22Apache%20Server%20Status%22%20inurl:%22/server-status%22%20-site:apache.org)
  * [Joomla form post assistant](https://google.com/search?q=allintitle:%22Forum%20Post%20Assistant%20:%22%20ext:php%20-site:joomla.org)
  * [phpinfo() - Zend scripting language engine](https://google.com/search?q=ext:php%20intext:%22Zend%20Scripting%20Language%20Engine%22%20-site:php.net%20-site:zend.com)
  * [phpinfo() - intitle](https://google.com/search?q=ext:php%20intitle:%22phpinfo()%22%20-site:php.net)
  * [phpinfo() - PHP Credit](https://google.com/search?q=ext:php%20intext:%22PHP%20Credits%22%20-site:php.net%20-site:github.com)

### Sensitive Files

  * [Facebook profile archive](https://www.google.com/search?q=inurl:%22html/security.htm%22%20intext:%22Active%20Sessions%22%20-github)

### Interesting Sites

  * [TurnKey LAMP stack](https://google.com/search?q=intitle:%22TurnKey%20LAMP%22%20intext:%22Resources%20and%20references%22)
