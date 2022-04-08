# Laravel 8
Install Laravel
```bash
composer create-project laravel/laravel example-app
```
Run Project
```bash
php artisan serve
```
Routing System
```bash
Route::get('/', [class_name::class, 'function_name']);
```

# Lumen API Documentation

## How to create a lumen api

Run this command to create your project

```bash
  composer create-project --prefer-dist laravel/lumen project_name
```
To Run the project Run this command

```bash
  php -S localhost:8000 -t public
```
## Install Command Generator on the project
Go to the follwing link and Read the documentation
https://github.com/flipboxstudio/lumen-generator
## API Authentication
Uncomment from your bootstrap/app.php
- $app->register(App\Providers\AuthServiceProvider::class);
- $app->routeMiddleware([  
     'auth' => App\Http\Middleware\Authenticate::class,  
 	]);
## What is JWT?
JWT is JSON web token for encrypt to decrypt JSON File for json file secure transform and 
this is not a library, it's like a proccess.  
JWL Official address https://jwt.io/  
PHP library for JWT https://github.com/firebase/php-jwt
### How to Install JWT
Create a folder on localhost root folder for JWT  
You Must add this 3 line
```bash
  use Firebase\JWT\JWT;
  use Firebase\JWT\Key;
  include 'vendor/autoload.php';
```
## Laravel | Front-end Scaffolding
Front-end Scaffolding means to create a basic structure for an application. Laravel provides a very simple way to change the front-end presets/scaffolding with any of the other available scaffolding like Bootstrap, Vue and React.
First of all you have to install ui package by this command
```bash
composer require laravel/ui
```
Generate basic scaffolding...
 ```bash
 php artisan ui bootstrap
 php artisan ui vue
 php artisan ui react
 ```
 Genarate scaffolding with login/registration 
   ```bash
   php artisan ui bootstrap --auth
   php artisan ui vue --auth
   php artisan ui react --auth
   ```
   And now run this command
   ```bash
   npm install
   ```
Now run another command for load bootstrap style. Note: You should run this command 2 times.
```bash
npm run dev
```
## Setup React Bootstrap
Run the command in your project
```bash
npm install react-bootstrap bootstrap
```
Official address for react bootstarp is https://react-bootstrap.github.io/
