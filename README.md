# Setup for virgin environment

The project consists of two components which requires four steps to setup.

1. Import all files and folders from the .zip file inside a PHP accessible webpath (e.g. XAMP’s _/htdocs_)
2. Inside MySQL, create a new database with utf-8 collation. (E.g. boatie_db)
3. Inside MySQL, create a new user that has unrestricted access to the newly created database only (look at the boatie_admin code snippet from 4.5).
4. Open the file _/config/db-config.php_ and update all credentials to your environment.
5. Import the sql_dump.sql that can be found inside the backup folder.

That’s it. Now you should be able to visit the working project at \*localhost/project_folder/**public\*** .
To access the dashboard, visit \*localhost/project_folder/**public/dashboard\*** and log in with the admin account:
Account: max@boatie.dk
Password: hello123

For the curious people, the deployed web version doesn’t require the www.example./public path as /public has been specified as the webroot using .htaccess
