#How to use

__General__
- `git clone`- Clone the repository

__Backend__
- `cd backend` - Go to the folder with backend api
- `cp .env.example .env` - Copy the file and edit credentials for a database MySQL
- `composer install`
- `php artisan key:generate`
- `php artisan migrate --seed` - Create tabels in database and add some data for testing
- `php artisan serve` - Run server for the backend

__Frontend__
- `cd frontend` - Go to the folder with frontend client
- `npm install`
- `npm run serve` - Run server for the frontend
