# Laravel Team_Project Docker 
<p>based on development build: Finish TEAM-88_Layout_edit</p>
<p>Problems:</p>
<p>Performance (not sure if on browser side or server, tho resource usage seems to be normal)</p>

# How to use:

## Change .env db setting to:

<p>DB_CONNECTION=mysql</p>
<p>DB_HOST=db</p>
<p>DB_PORT=3306</p>
<p>DB_DATABASE=laravel</p>
<p>DB_USERNAME=root</p>
<p>DB_PASSWORD=123456</p>

<p>after that run fallowing commands:</p>
<p>docker-compose build --no-cache</p>
<p>docker-compose up</p>

## Migrations 
<p>in docker desktop open cil console for laravel/app and run fallowing commands:</p>
<p>php artisan migrate</p>

## if you get error "file_put_contents(path): failed to open stream: No such file or directory"
<p>first got to public folder and delete folder called "storage" than in docker desktop open cil console for laravel/app and run fallowing commands:</p>
<p>composer dump-autoload</p>
<p>composer install</p>
<p>php artisan clear-compiled</p>
<p>php artisan config:clear</p>


