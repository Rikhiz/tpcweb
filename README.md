git clone https://github.com/Rikhiz/tpcweb.git
cd tpcweb
composer install
cp .env.example .env
php artisan key:generate
npm install

.env  Ganti ->
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=tpcdb
DB_USERNAME=root
DB_PASSWORD=

(Jika sudah membuat kerangka database)
php artisan migrate

Jalanin BackEnd
php artisan serve
npm run dev
