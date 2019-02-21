# Quicktext App Documentation
## Introduction  
Quicktext™ is a channel manager of instant communications that combines SMS, instant messaging and live chat in the same interface connected to the PMS.

## Documentation

This project hosts the documentation available at http://www.xxxxx.xx/.


## Requirements

- PHP >= 5.6
- The PHP IMAP extension
- Node.js, NPM & GULP

## Get Started

Clone the repository and install the dependencies

```sh
$ git clone git@gitlab.satoripop.tn:quicktext/quicktext.git
$ cd quicktext
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


## Version 3.0

Run following sql:

```sh
UPDATE `im_message_meta` SET `date`=`date`*1000 WHERE `date`<10000000000
UPDATE `im_archived_message_meta` SET `date`=`date`*1000 WHERE `date`<10000000000

UPDATE `im_message_meta` SET `trigger`= 2 WHERE `trigger`= 0
UPDATE `im_archived_message_meta` SET `trigger`= 2 WHERE `trigger`= 0
```