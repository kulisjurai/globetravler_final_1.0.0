# globetravler_final_1.0.0
Final exam application for IT Academy program Javascript Frontend development 2021. Subject of the work is traveling and booking agency.

## Node version

````npm .nvmrc**```` file can be found in the ````npm api```` folder with the version of node required for the project.

## Data base

If the project was downloaded using the git clone command the exportded dump **globetraveler_dump.sql** file should be at the same location as the **api** and **client** folders are.
Copy the __globetraveler_dump.sql__ file into your __bin__ directory (subdirectory of MySql Server) and in the same directory (__bin_) type following command:

```mysql
mysql -u "type-your-username" -p "type-your-newly-created-database_name" < globetraveler_dump.sql
```


### Configure database in .env file

In the **api** folder there is an **.env** file which contain basic configuration data for the project. Type
newly created database (step above) informations for DB_HOST, DB_DATABASE, DB_USER, DB_PASSWORD.

example:

```.env
DB_HOST=localhost
DB_DATABASE=globetravelers
DB_USER=root
DB_PASSWORD=password
```

## Mail sender

For sending emails we are using https://mailtrap.io/ with Nodemailer. Sign up for the account and set required variables in **.env** file:

```.env
SMTP_HOST=smtp.mailtrap.io
SMTP_PORT=2525
SMTP_USERNAME=you-will-get-this-after-sign-up
SMTP_PASSWORD=you-will-get-this-after-sign-up
```

## Application start

In **api** and **client** folders type following command: `npm install`

To start the app use `npm start` command for the **api** folder and `ng serve` for the **client** folder.
