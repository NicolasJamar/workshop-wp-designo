# Workshop WordPress

## Intro

In this workshop you will learn the basics of WordPress by creating a custom theme. That means, you will not only deal with the dashboard & add content, but organize your own theme with custom templates. 

## Chapters

- [Installation](#install)
- Overview the dashboard
- Activate the custom theme
- Pages templates
- The templates hierarchy
- Menu creation
- The Codex
- Custom Posts
- Advanced custom fields
- Images
- Categories
- Going further

## [Installation][install]

Once you have launch your environment (a server with PHP & MySQL), you're ready to start. 

The first thing to do is to create an empty database in your DB manager. Git it a name. 

The next step is to go the file ``wp-config.php` & write the correct info of your DB to be able to link it with WorkPress.  

```php
// ** MySQL settings - You can get this info from your web host ** //
/** The name of the database for WordPress */
define('DB_NAME', 'designo');

/** MySQL database username */
define( 'DB_USER', 'root' );

/** MySQL database password */
define( 'DB_PASSWORD', 'password' );

/** MySQL hostname */
define( 'DB_HOST', 'mysql' );

```

> 👉 To allow plugins to be installed on Linux, you may write the following line in your `wp-config.php` file : `define('FS_METHOD','direct');`

---

## The Docker installation

### What is this ?
This template repository is a boilerplate setup for a PHP application.

Its current version ships with PHP 8.1, Mysql 8.0, phpMyAdmin and an Nginx server running on Alpine.
All of it orchestrated and run by Docker Compose.

### Requirements
Docker Engine and Docker Compose

### How to use it ?
Clone this repository, or click the _Use this template_ button on Github.
For more information about Github repositories, please refer to the [Github documentation](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template).

Once cloned, please refer to the README.md file provided by phpdocker.io in the phpdocker directory to run the application.

The entrypoint of your php application will be _/src/public/index.php_.

### Notes
The Docker Compose file was _initially_ generated by [phpdocker.io](https://phpdocker.io/).
