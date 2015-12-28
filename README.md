# nginx-source

Installs [NGINX](https://www.nginx.com/resources/wiki/) from source on CentOS ```6.x``` and ```7.x``` operating systems.

### NGINX Version

This script will install the latest stable version of nginx, currently ```1.8.0```, by default. That being said, any version of NGINX can be specified for installation using the ```-v``` switch followed by the desired version.

current version ```1.8.0```

### NGINX Modules

By default the following modules are included with this installation:

- [http_gzip_static_module](http://nginx.org/en/docs/http/ngx_http_gzip_static_module.html) - gzip compression support
- [http_realip_module](http://nginx.org/en/docs/http/ngx_http_realip_module.html) - x-forwarded-for http header support
- [http_stub_status_module](http://nginx.org/en/docs/http/ngx_http_stub_status_module.html) - http error code substatus support
- [http_ssl_module](http://nginx.org/en/docs/http/ngx_http_ssl_module.html) - https support
- [pcre](http://www.pcre.org/) - perl compatible regular expression support

### Installation

Usage:

```
  Usage: ./install -(i|u)

    -i        install nginx from source
    -u        uninstall nginx
    -v        install specific nginx version (default: 1.8.0)
```  

Installation:

```
$ git clone git@github.com:audio4ears/nginx-source.git
$ nginx-source/install
```
