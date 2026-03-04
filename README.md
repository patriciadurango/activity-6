# Activity 6 — Laravel Artisan Command Console

A Laravel project built to explore and apply the Artisan command-line interface. The project scaffolds a Product resource including its model, migration, resource controller, and Blade views.

## What this project covers

- Generating an application key
- Running a local development server
- Creating symbolic links for file storage
- Scaffolding models, controllers, migrations, seeders, and factories
- Working with resource controllers and RESTful routing
- Running, rolling back, and refreshing database migrations

## Project structure

```
app/
  Models/Product.php
  Http/Controllers/ProductController.php
database/
  migrations/create_products_table.php
resources/
  views/products/
    show.blade.php
    edit.blade.php
    create.blade.php
```

## Setup

```bash
composer install
cp .env.example .env
php artisan key:generate
php artisan migrate
php artisan serve
```

## Key commands used

```bash
php artisan make:model Product -mc --resource
php artisan make:seeder ProductSeeder
php artisan make:factory ProductFactory
php artisan route:list
php artisan migrate:fresh --seed
```

