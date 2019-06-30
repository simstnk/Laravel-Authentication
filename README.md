<p align="center"><img src="https://www.5balloons.info/wp-content/uploads/2017/10/Screen-Shot-2017-10-02-at-1.47.12-PM.png"></p>

## Laravel-Authentication Login, Logout, Register, Forgot Password & Remember Me Functionality
Laravel framework comes with an out of box working authentication functionality for your application that includes Login, Logout, Register, Forgot Password and Remember me functions.

## Requirements
>Working Laravel Framework (I am using Laravel 5.8)
> >MySQL with database created to be used by your application.
> > >Configuration changes in .env file to set database properties.

### Step 1 : Laravel Installation
Make sure you have a working Laravel application on your machine. Also you have configured your .env file as per the database you are using. Once you have installed laravel. It should have the following folder structure. As you can see Laravel application already have some classes that are specific to the Authentication functionality. Controller that are specific to the authentication module are under app > Controllers > Auth:    

- [Laravel Framework](https://github.com/laravel/framework)
- [Laravel Documentation](https://laravel.com/docs)
- [Laracasts](https://laracasts.com)


### App Service Provider
    To avoid errors, in the AppServiceProvider file add:
> use Illuminate\Support\Facades\Schema;

    Also change the Bootstrap any application services:
> Schema::defaultStringLength();

### node modules
Node modules was installed:
> npm install

### Step 2 : Run make:auth command
On your project root directory run following command.
> php artisan make:auth

### Step 3 : Run migrate command
Next, we need to run the migrate command to create the tables required for authentication. Run the following command on project Root in your terminal.
> php artisan migrate
