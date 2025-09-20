<h1 align="center">
 Docker File from php8.2  <br>
 (Laravel, Symfony, Wordpress, etc..)
</h1>


![Packagist PHP Version Support](https://img.shields.io/badge/php-%5E8.2-blue)


Docker file for use in PHP Symfony support for php XX.
- Laravel
- PhpCake.
- Wordpress.
- Drupal.
- etc.




## 🚀 Installation
### From Docker File.

In your terminal in same folder you down dockerfile execute this sentences.
```terminal
docker build -t /php_fpmXX_nginx .
docker run -p 9000:9000  --name php_fpmXX_nginx php_fpmXX 
```

## :arrow_forward: How to use.
In your web server to use this container add the proxy pass for example:.
### Apache.
```conf
ProxyPassMatch ^/(.*\.php(/.*)?)$ fcgi://php_fpmXX:9000/var/www/html/public/$1
```

## :mag_right: Change log
Please see <a href="">CHANGELOG</a> for more information what has changed recently.



## :superhero_woman: Contribute.
Feel free to make as many pull requests as you think fit, because there are so many things to do, all help is welcome.

Here is a guide if you want to take a look()

If you find a bug, let us know <a href="">here</a> .

If you request a new  <a href =""> feature</a>.
