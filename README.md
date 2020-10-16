# WPStarter boilerplate

Bootstraping a new website application with WordPress based on [WPStarter](https://github.com/wecodemore/wpstarter).

## Usage

Fetching the boilerplate via composer to a new directory (`my-website`):

```
$ composer create-project inpsyde/wpstarter-boilerplate:dev-master my-website
```
You will get asked if you want to remove the existing git history. Answer with _yes_ (Y) as you're about to start a new project.

That will give you the following directory structure:

```
[my-website]
 ├ public/
 | ├ wp/
 | ├ wp-content/
 | | ├ plugins/
 | | └ themes/
 | ├ index.php
 | └ wp-config.php
 ├ vendor/
 ├ .env.example
 ├ .gitignore
 ├ composer.json
 ├ composer.lock
 └ README.md
```

**Web server configuration**

Configure your web server to use the directory `public/` as document root (web root).

**Steps to take**

* If using Apache web server, copy `templates/.htaccess.example` to `public/.htaccess`.
* Copy `templates/.env.example` to `.env` and set the required database credentials and `WP_HOME` in the `.env` file.

