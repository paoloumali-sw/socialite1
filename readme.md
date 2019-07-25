# socialite1

## server setup
- $ ``sudo apt install -y nginx php-memcached php-msgpack php-igbinary $(php_pack=(fpm cli gd mysql pgsql imap mbstring xml curl bcmath sqlite3 soap intl readline imagick zip yaml);printf 'php7.2-%s ' "${php_pack[@]}")``

## local dev

- clone [paoloumali-sw/socialite1](https://github.com/paoloumali-sw/socialite1)
- $ ``composer install``
- $ ``ln -s $(pwd)/.env.example .env`` or ``cp .env.example .env``
- $ ``touch database/database.sqlite``
- $ ``php artisan migrate``
- $ ``php artisan serve``

## db seeding

- $ ``php artisan migrate:refresh --seed``

## tuts

- https://medium.com/employbl/add-login-with-google-to-your-laravel-app-d2205f01b895