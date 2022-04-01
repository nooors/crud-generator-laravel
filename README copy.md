<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400"></a></p>

<p align="center">
<a href="https://travis-ci.org/laravel/framework"><img src="https://travis-ci.org/laravel/framework.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
</p>

## About this exercice

composer create-project laravel/laravel:"8*" project-name

## Create Database

## Conig .env whith Data Base credentials

## Make migration in order to create a migration

php artisan make:migration libros

## In database\migration the migration recently created

Schema::create('<table>', function (Blueprint $table)){
## Create table fields
        $table->bigIncrements('id);
        $table->string ('nombre);
        $table->decimal('precio);
## etc
}

## migrate the migrations to write in db the possible changes between bd and migrations

php artisan migrate

# create a bootstrap interface that allow the user login or register

composer require laravel/ui

php artisan ui bootstrap --auth

npm install

npm run dev

## Install CRUD generator

composer require ibex/crud-generator --dev

php artisan vendor:publish --tag=crud

## create crud for libros model
## Create Controller
## Create Model
## Create views
php artisan make:crud libros

## Protect route with a middleware

Route::resource (.............)->middleware('auth')




