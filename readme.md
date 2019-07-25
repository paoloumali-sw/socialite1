# socialite1

## server setup
- $ ``sudo apt install -y nginx php-memcached php-msgpack php-igbinary $(php_pack=(fpm cli gd mysql pgsql imap mbstring xml curl bcmath sqlite3 soap intl readline imagick zip yaml);printf 'php7.2-%s ' "${php_pack[@]}")``

## local dev

- $ ``ln -s $(pwd)/.env.example .env``
- $ ``php artisan serve``