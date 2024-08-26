# SimpleAuthApp

This is a simple web application built using PHP Laravel and Bootstrap. The application includes basic login and registration functionality with form validation and error handling.

## Stack

- **Backend**: PHP Laravel
- **Frontend**: Bootstrap 4
- **Database**: MySQL

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/GIKS-India-Private-Limited/ProjectDemo.git
    cd SimpleAuthApp
    ```

2. Install dependencies:
    ```bash
    composer install
    npm install
    ```

3. Create a `.env` file from the `.env.example` file and configure your database settings:
    ```bash
    cp .env.example .env
    ```

4. Generate an application key:
    ```bash
    php artisan key:generate
    ```

5. Run migrations:
    ```bash
    php artisan migrate
    ```

6. Compile the assets:
    ```bash
    npm run dev
    ```

7. Serve the application:
    ```bash
    php artisan serve
    ```

    Visit `http://localhost:8000` to view the application.

## Code Structure

- **app/Http/Controllers/Auth**: Contains the authentication controllers (LoginController, RegisterController, etc.).
- **resources/views/auth**: Contains the views for authentication (login, register, password reset).
- **routes/web.php**: Defines the web routes for the application.
- **database/migrations**: Contains the migration files for creating database tables.

## Design Decisions

- **Laravel UI**: Chose Laravel UI for quickly scaffolding authentication with Bootstrap support.
- **Form Validation**: Leveraged Laravel's built-in form validation to ensure data integrity and provide feedback to users.
- **Bootstrap**: Used Bootstrap for styling the authentication pages, making them responsive and visually appealing.

## Future Improvements

- Add email verification.
- Implement password reset functionality.
- Customize the UI further with additional Bootstrap components.