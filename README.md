
# Ospek Unida 2024 Laravel Application

## Requirements

Before running the application, make sure you have the following installed on your system:

- PHP 8.3 or higher
- Composer
- MySQL or another supported database
- Node.js and npm (for frontend assets)
- Laravel 10.x

## Installation

Follow these steps to set up the application:

### 1. Clone the Repository

Clone the repository to your local machine:

```bash
git clone https://ospek_unida_2024.git
cd ospek_unida_2024
```

### 2. Install Dependencies

Install PHP dependencies using Composer:

```bash
composer install
```

### 3. Set Up Environment File

Copy the `.env.example` file to `.env`:

```bash
cp .env.example .env
```

### 4. Generate Application Key

Run the following command to generate the application key:

```bash
php artisan key:generate
```

### 5. Install Frontend Dependencies

Install JavaScript and CSS dependencies using npm:

```bash
npm install
```

### 6. Run Migrations

Run the database migrations:

```bash
php artisan migrate
```

If you want to refresh the database and re-seed:

```bash
php artisan migrate:fresh --seed
```

### 7. Serve the Application

Run the application using the built-in Laravel server:

```bash
php artisan serve && npm run dev
```

Your application should now be running at `http://127.0.0.1:8000`.

## Additional Commands

- Run tests: `php artisan test`
- Clear cache: `php artisan cache:clear`
- Queue listener: `php artisan queue:work`

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.
