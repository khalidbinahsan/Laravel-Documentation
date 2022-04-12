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
## What is Axios?
Axios is a promise-based HTTP Client for node.js and the browser. It is isomorphic (= it can run in the browser and nodejs with the same codebase).   On the server-side it uses the native node.js http module, while on the client (browser) it uses XMLHttpRequests.
Official website for Axios is: https://axios-http.com/
Axios is javascript library for Http client
## Jquery in Laravel
If Jquery not working on laravel project load this CDN at head of Layout.app.blade.php file
```bash
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/4.1.3/css/bootstrap.min.css" />
    <script src="http://ajax.googleapis.com/ajax/libs/jquery/1.9.1/jquery.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/bootstrap-3-typeahead/4.0.1/bootstrap3-typeahead.min.js"></script>
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
