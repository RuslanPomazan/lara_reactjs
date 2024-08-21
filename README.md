
# Laravel Docker Starter Kit
- Laravel v11.9
- PHP v8.2.10
- MySQL v8.1
- MariaDB v10.11
- Mailpit v1.8.4
- Node.js v18.17.1
- NPM v10.1.0
- Yarn v1.22.19
- Vite v4.4.9

# Requirements
- Stable version of [Docker](https://docs.docker.com/engine/install/)
- Compatible version of [Docker Compose](https://docs.docker.com/compose/install/#install-compose)

# How To Deploy

### For first time only !
- `docker-compose up -d`
- `docker-compose exec php bash`
- `composer setup`

### From the second time onwards
- `docker-compose up -d`
- `docker-compose exec php bash`

# Notes

### Basic docker compose commands
- Build or rebuild services
    - `docker-compose build`
- Create and start containers
    - `docker-compose up -d`
- Stop and remove containers, networks
    - `docker-compose down`
- Stop all services
    - `docker-compose stop`
- Restart service containers
    - `docker-compose restart`
- Run a command inside a container
    - `docker-compose exec [container] [command]`

### Useful Laravel Commands
- Display basic information about your application
    - `php artisan about`
- Remove the configuration cache file
    - `php artisan config:clear`
- Flush the application cache
    - `php artisan cache:clear`
- Clear all cached events and listeners
    - `php artisan event:clear`
- Delete all of the jobs from the specified queue
    - `php artisan queue:clear`
- Remove the route cache file
    - `php artisan route:clear`
- Clear all compiled view files
    - `php artisan view:clear`
- Remove the compiled class file
    - `php artisan clear-compiled`
- Remove the cached bootstrap files
    - `php artisan optimize:clear`
- Delete the cached mutex files created by scheduler
    - `php artisan schedule:clear-cache`
- Flush expired password reset tokens
    - `php artisan auth:clear-resets`

### Laravel Pint (Code Style Fixer | PHP-CS-Fixer)
- Format all files
    - `./vendor/bin/pint`
- Format specific files or directories
    - `./vendor/bin/pint app/Models`
    - `./vendor/bin/pint app/Models/User.php`
- Format all files with preview
    - `./vendor/bin/pint -v`
- Format uncommitted changes according to Git
    - `./vendor/bin/pint --dirty`
- Inspect all files
    - `./vendor/bin/pint --test`

# TODO
- Improve environment
- Add more containers

---

## About Laravel

Laravel is a web application framework with expressive, elegant syntax. We believe development must be an enjoyable and creative experience to be truly fulfilling. Laravel takes the pain out of development by easing common tasks used in many web projects, such as:

- [Simple, fast routing engine](https://laravel.com/docs/routing).
- [Powerful dependency injection container](https://laravel.com/docs/container).
- Multiple back-ends for [session](https://laravel.com/docs/session) and [cache](https://laravel.com/docs/cache) storage.
- Expressive, intuitive [database ORM](https://laravel.com/docs/eloquent).
- Database agnostic [schema migrations](https://laravel.com/docs/migrations).
- [Robust background job processing](https://laravel.com/docs/queues).
- [Real-time event broadcasting](https://laravel.com/docs/broadcasting).

Laravel is accessible, powerful, and provides tools required for large, robust applications.

## Learning Laravel

Laravel has the most extensive and thorough [documentation](https://laravel.com/docs) and video tutorial library of all modern web application frameworks, making it a breeze to get started with the framework.

You may also try the [Laravel Bootcamp](https://bootcamp.laravel.com), where you will be guided through building a modern Laravel application from scratch.

If you don't feel like reading, [Laracasts](https://laracasts.com) can help. Laracasts contains over 2000 video tutorials on a range of topics including Laravel, modern PHP, unit testing, and JavaScript. Boost your skills by digging into our comprehensive video library.
