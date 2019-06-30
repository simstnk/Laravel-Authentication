<p align="center"><img src="https://i.stack.imgur.com/3yJyt.png"></p>

### Laravel Authentication Login, Logout, Register, Forgot Password & Remember Me Functionality
Laravel framework comes with an out of box working authentication functionality for your application that includes Login, Logout, Register, Forgot Password and Remember me functions.

### Requirements 
    Working Laravel Framework (I am using Laravel 5.8)
    MySQL with database created to be used by your application.
    Configuration changes in .env file to set database properties.
    
### Step 1 : Laravel Installation
Make sure you have a working Laravel application on your machine. Also you have configured your .env file as per the database you are using. Once you have installed laravel. It should have the following folder structure.
 Laravel application already have some classes that are specific to the Authentication functionality. Controller that are specific to the authentication module are under app > Controllers > Auth
 
 ### App Service Provider:
 To aviod errores, in the file provider make changes to the AppServiceProvider.php:
 > use Illuminate\Support\Facades\Schema;
 >> Schema::defaultStringLength();
>>> However, the changes have been corrected.

### node Modules:
Node modules was add to the file structure:
> npm install

### Step 2 : Run make:auth command:
On your project root directory run following command.
>php artisan make:auth

### Step 3 : Run migrate command:
Next, we need to run the migrate command to create the tables required for authentication. Run the following command on project Root in your terminal.
> php artisan migrate

### How To:
The step above is already configured for you all you have to do is configure the .env file to your server and database. Howerver, if you want to start a fresh install follow the steps above.
