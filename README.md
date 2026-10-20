# Real-Time Chat Application

A Laravel practice project exploring real-time chat functionality with Laravel Reverb and Livewire.

## Tech Stack

- PHP 8.2+
- Laravel 11
- Laravel Reverb
- Livewire 3
- Livewire Volt
- Laravel Breeze
- Vite

## Features

- Authenticated chat page
- Chat rooms accessed by slug
- Real-time messaging using Laravel Reverb

Confirm that message persistence, room membership rules, and private-channel authorization match the current implementation before documenting them as supported features.

## Requirements

- PHP 8.2 or later
- Composer
- Node.js and npm
- A supported database

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/Sadeghjamali/Larachat-reverb.git
   cd Larachat-reverb
   ```

2. Install dependencies:

   ```bash
   composer install
   npm install
   ```

3. Create the environment file and generate the application key:

   ```bash
   cp .env.example .env
   php artisan key:generate
   ```

4. Configure your database and run migrations:

   ```bash
   php artisan migrate
   ```

5. Configure Laravel Reverb and broadcasting in `.env` using the values required by your local setup. Do not commit real credentials.

6. Build frontend assets:

   ```bash
   npm run build
   ```

7. Start the Laravel development server:

   ```bash
   php artisan serve
   ```

8. In a separate terminal, start the Reverb server:

   ```bash
   php artisan reverb:start
   ```

For local development, use the environment variables and host/port settings that match your Reverb and broadcasting configuration.

## Testing Real-Time Messaging

Open the application in two separate authenticated browser sessions and verify that a message sent from one session appears in the other without manually refreshing the page.

## Notes

This is a learning project. Verify authentication, room access, broadcasting authorization, and message persistence before describing these behaviors as production-ready.

## Repository

https://github.com/Sadeghjamali/Larachat-reverb
