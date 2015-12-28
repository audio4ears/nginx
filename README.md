# nginx-source

Installs [NGINX](https://www.nginx.com/resources/wiki/) from source on CentOS ```6.x``` and ```7.x``` operating systems.

### NGINX Version

This script will keep its default version of NGINX inline with the default version being utilized by the Chef Supermarket [NGINX](https://supermarket.chef.io/cookbooks/nginx) Cookbook. That being said, any version of NGINX can be specified for installation using the ```-v``` switch followed by the desired version.

default version: ```1.6.2```

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
  Usage: ./install -(install|uninstall)

    -i|install        install nginx from source
    -u|uninstall      uninstall nginx
    -v|version        install specific nginx version (default: 1.6.2)
```  

Installation:

```
$ git clone git@github.com:audio4ears/nginx-source.git
$ nginx-source/install
```

Custom Installation:

```
$ git clone git@github.com:audio4ears/nginx-source.git
$ nginx-source/install -v 1.2.3
```
