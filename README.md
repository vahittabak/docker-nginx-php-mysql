# Dockerise your Wordpress blog with Nginx, PHP7-FPM and MySQL

### Step 1:
Download Wordpress latest version
* [https://wordpress.org] [DlWp]

### Step 2:
Replace the downloaded wordpress folder with the empty wordpress folder

### Step 3:
Change wp-config-sample.conf file name as wp-config.conf.
Edit wp-config file, your updated wp-config.conf shoul look like this;
```sh
// ** MySQL settings - You can get this info from your web host ** //
/** The name of the database for WordPress */
define('DB_NAME', 'website_db');

/** MySQL database username */
define('DB_USER', 'website_user');

/** MySQL database password */
define('DB_PASSWORD', 'strong_password');

/** MySQL hostname */
define('DB_HOST', 'db:3306');

/** Database Charset to use in creating database tables. */
define('DB_CHARSET', 'utf8');

/** The Database Collate type. Don't change this if in doubt. */
define('DB_COLLATE', '');
```

### Step 4:
Finally, run docker-compose
```sh
$ docker-compose build
$ docker-compose up
```

### Step 5:
Test the result. Wordpress setup file should be available on 
* [http://localhost:8080] [Local]
