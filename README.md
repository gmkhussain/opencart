#Configuration setting on server

## Open Config.php file

```html
<?php
// HTTP
define('HTTP_SERVER', 'http://ABCXYZ.com/public_html/');
define('HTTP_IMAGE', 'http://ABCXYZ.com/public_html/image/');
define('HTTP_ADMIN', 'http://ABCXYZ.com/public_html/admin/');

// HTTPS
define('HTTPS_SERVER', 'http://ABCXYZ.com/public_html/');
define('HTTPS_IMAGE', 'http://ABCXYZ.com/public_html/image/');

// DIR
define('DIR_APPLICATION', '/home/XXXX/public_html/catalog/');
define('DIR_SYSTEM', '/home/XXXX/public_html/system/');
define('DIR_DATABASE', '/home/XXXX/public_html/system/database/');
define('DIR_LANGUAGE', '/home/XXXX/public_html/language/');
define('DIR_TEMPLATE', '/home/XXXX/public_html/view/template/');
define('DIR_CONFIG', '/home/XXXX/public_html/system/config/');
define('DIR_IMAGE', '/home/XXXX/public_html/image/');
define('DIR_CACHE', '/home/XXXX/public_html/system/cache/');
define('DIR_DOWNLOAD', '/home/XXXX/public_html/download/');
define('DIR_LOGS', '/home/XXXX/public_html/system/logs/');

// DB
define('DB_DRIVER', 'mysql');
define('DB_HOSTNAME', 'localhost');
define('DB_USERNAME', 'XXXX_usr');
define('DB_PASSWORD', 'XXXXXXXXX');
define('DB_DATABASE', 'XXXX_db');
define('DB_PREFIX', 'oc_');?>
```







##How to add a Information page link into navigation
```html
<li><a class="<?php if ((isset($this->request->get['route']) && $this->request->get['route']=="information/information") && (isset($this->request->get['information_id']) && $this->request->get['information_id']=="13")) {echo "active";} ?>" href="index.php?route=information/information&information_id=4"><i class="icon-bug"></i>Test</a></li>
```