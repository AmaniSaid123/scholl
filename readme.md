# Scholl App Documentation
## Introduction  
Scholl™ is a .

## Documentation

This project hosts the documentation available at http://www.xxxxx.xx/.


## Requirements

- PHP >= 5.6
- The PHP IMAP extension
- Node.js, NPM & GULP

## Get Started

Clone the repository and install the dependencies

```sh
$ git clone git@github.com:AmaniSaid123/scholl.git
$ cd scholl
$ composer install
$ php artisan key:generate

# before running 'php artisan migrate' you should create the database
# This package ships with a .env.example file
# in the root of the project.
# You must rename this file to just .env
# Note: Make sure you have hidden files shown on your system

$ php artisan migrate
$ php artisan laroute:generate
$ php artisan storage:link
$ npm install

```
If you need help installing the project, please contact the .

If you've instead found a bug  or would like new features added, go ahead and open issues or pull requests against this repo!
#### NB : RUN 'php artisan laroute:generate' when ever the web.php (routes) file is updated

