Laravel Blog Application
Description
This is a simple blog application built using Laravel. Users can create, edit, and delete their own blog posts. An admin can manage users and their posts.

Features
User Registration & Authentication
Blog Post Creation, Editing, and Deletion
Admin Functionality for user and post management
Pagination for blog posts
Search functionality to find posts by title or content
Requirements
PHP >= 7.4
Composer
Laravel >= 8.0
SQLite3
Installation
1. Clone the Repository
git clone https://github.com/Harshakottur/Laravel_blog-app.git
cd Laravel_blog-app
2. Install Composer Dependencies
composer install
3. Set Up SQLite Database
Create a new SQLite database file:

Navigate to your project directory and create a database file:
touch database/database.sqlite
(For Windows, use echo. > database\database.sqlite)

Update your .env file:

DB_CONNECTION=sqlite
DB_DATABASE=/absolute/path/to/your/project/database/database.sqlite
Replace /absolute/path/to/your/project/ with the actual path to your Laravel project.

4. Run Migrations and Seeders
php artisan migrate --seed
This command will create the necessary database tables and insert the admin user defined in the AdminSeeder.php.

5. Start the Development Server
php artisan serve
Your application will be running at http://localhost:8000.

RUN Seeder File Migration for Admin LOGIN
php artisan db:seed --class=AdminSeeder
Usage
Navigate to the application in your web browser and use the admin credentials to log in:
Email: admin@example.com
Password: password
Contributing
Feel free to submit pull requests for any improvements or features!

License
This project is open-source and available under the MIT License.