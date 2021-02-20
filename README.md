# Findlancer repository - A marketplace like upwork.

## Dependencies required

To use this repository, you must first ensure that
these dependencies below are already installed.
Make sure your server meets the following requirements:

- [tmux](https://doc.ubuntu-fr.org/tmux) (For multi window in terminal - NB: Linux or Mac)
- [Node.js](https://nodejs.org/)
- [yarn](https://yarnpkg.com)
- [maildev](https://danfarrelly.nyc/MailDev/)
- [Laravel Requirements](https://laravel.com/docs/5.8#server-requirements)
- [make](http://www.gnu.org/software/make/) - (Already installed on Linux)
- [composer](https://getcomposer.org/download/)
- [elasticsearch](https://www.elastic.co/fr/elasticsearch/)
- Database (Mysql/Others)

## Usage

Clone the repository first.

``` bash
$ git clone https://Moussa-Ball@bitbucket.org/uplancecanada/uplance.git
```

Rename the .env.example file to .env and configure the environment variables 
by adding also these variables below and their values.

Do not forget to configure the variables for the database and the email.
After configuring the environment variables, proceed as follows in the terminal.

NB: Linux/Mac

``` bash
$ composer install
$ yarn install
$ php artisan migrate
$ make dev
```

:warning Do not make `make dev` on windows if you dont have installed `make` and `tmux`.
Use [cmder](https://cmder.net/) and launch on each tab the commands below.
Do the above steps without make dev then do what is mentioned below.

``` bash
$ php artisan serve
$ yarn hot or npm run hot
$ maildev --ip 127.0.0.1
```

If you have a 404 problem or 500 with apache. Refer to this link below to solve the problem.

### [404 Error | Laravel - Apache](https://stackoverflow.com/questions/22757749/laravel-redirects-to-a-route-but-then-apache-gives-404-error)

### [500 Error | Laravel - Apache](https://stackoverflow.com/questions/31543175/getting-a-500-internal-server-error-on-laravel-5-ubuntu-14-04)
