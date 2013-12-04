# OpenShift Nginx Magento Cartridge
This cartridge serves static content using nginx web server, passing requests to .php files down to php-fpm.

## Usage

Create a magento app:

```bash
$ rhc app create magento https://reflector-getupcloud.getup.io/reflect?github=getupcloud/openshift-nginx-magento
```

For first steps instructions, please refer https://github.com/getupcloud/magento-scalable.


## User-defined configuration

Place your nginx .conf files inside config/nginx.d/. It will be include()ed from "server" scope.
Place your php-fpm .conf files inside config/php-fpm.d/. It will be include()ed from main php-fpm.conf file.
