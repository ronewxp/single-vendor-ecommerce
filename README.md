# Getting started

​

## Installation

​

Please check the official laravel installation guide for server requirements before you start. [Official Documentation](https://laravel.com/docs/8.x)

​

Alternative installation is possible without local dependencies relying on [Docker](#docker). 

​

Clone the repository

​

    git clone https://github.com/ronewxp/single-vendor-ecommerce.git
​

Switch to the repo folder

​

    cd single-vendor-ecommerce

​

Install all the dependencies using composer

​

    composer install

​

Copy the example env file and make the required configuration changes in the .env file

​

    cp .env.example .env

​

Generate a new application key

​

    php artisan key:generate

​

The Public Disk To create the symbolic link, you may use the storage:link Artisan command:

​

    php artisan storage:link
    
​

Run the database migrations (**Set the database connection in .env before migrating**)

​

    php artisan migrate --seed

​

Start the local development server

​

    php artisan serve
    
​
Start the local development server Host & Post

​

    php artisan serve --host=0.0.0.0 --port=8000

​

You can now access the server at http://localhost:8000 or http://127.0.0.1:8000 


**TL;DR command list**

​
 
    cp .env.example .env    

    composer install
    
    composer install --ignore-platform-req=php
    
    composer show -p
    
    composer update
    
    composer dump-autoload
    
    php artisan key:generate
    
        
​ NPM Comment 

    npm install
    
    npm run dev
    
    npm update
    
    npm cache clean --force
    

​ Artisan Migrate All Commend
    
    php artisan migrate --path='./database/migrations/2021_10_08_151109_create_appointments_table.php'
    
    php artisan migrate:rollback
    
    php artisan migrate:rollback --step=5
    
    php artisan migrate:reset
    
    php artisan migrate:refresh --seed
    
    php artisan migrate:fresh --seed
    
    php artisan db:seed
    
    php artisan db:seed --class=UserSeeder
    
    php artisan migrate:fresh --seed
    
    php artisan db:seed --force
    
    
   ​ Artisan All Clear Command
    
    php artisan cache:clear
    
    php artisan optimize
    
    php artisan route:clear
    
    php artisan view:clear
    
    php artisan config:clear
    

**Make sure you set the correct database connection information before running the migrations** [Environment variables](#environment-variables)

​

    php artisan migrate --seed

    php artisan serve
    
    php artisan serve --host=0.0.0.0 --port=8000
