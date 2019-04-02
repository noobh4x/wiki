# Workflow

## Recon

### Process

* Run `amass` to get a list of subdomains

> $ amass -d example.com -o amass.out

* Get a list of subdomains pointing to cloud services like aws, azure, github pages, etc using `cloudsub`

> $ cloudsub amass.out  
> sub.example.com  
> => foobar.cloudfront.com  
>  
> gh-pages.example.com  
> => banana.github.io  
> ...

### Tools

* [Amass](https://github.com/OWASP/Amass)
* [waybackurls](https://gist.github.com/noobh4x/9586bb9e74a9161359994c8a33196231) (Custom)
* [cloudsub](https://gist.github.com/noobh4x/4f904b99c3fd4c2ff9a2d75b3ba005c5) (Custom)
