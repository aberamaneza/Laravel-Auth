# Laravel Auth

A lightweight and scalable authentication system for Laravel, built with **PHP, Blade, and Laravel Web**.

Designed to be easy to integrate into an existing Laravel project by simply copying the authentication files and registering the provided routes.

## Features

* 🔐 Authentication system
* 📧 Email verification
* 🔢 OTP verification via email
* 🔑 Password reset
* 📩 Email sending
* 🧩 Blade-based authentication views
* ⚡ Built with Laravel Web + PHP
* 📈 Scalable architecture
* 🛠️ Easy to extend with additional fields and authentication features

## Installation

### 1. Copy the files

Copy the authentication files from this repository into your Laravel project while keeping the same directory structure.

### 2. Register the authentication routes

Open your Laravel `routes/web.php` file and include the provided `auth.php` routes:

```php
require __DIR__.'/auth.php';
```

### 3. Run migrations

After copying the migration files, run:

```bash
php artisan migrate
```

### 4. Configure email

Configure your Laravel mail settings in `.env` so the application can send verification and OTP emails.

Example:

```env
MAIL_MAILER=smtp
MAIL_HOST=your-smtp-host
MAIL_PORT=587
MAIL_USERNAME=your-email
MAIL_PASSWORD=your-password
MAIL_ENCRYPTION=tls
MAIL_FROM_ADDRESS="your@email.com"
MAIL_FROM_NAME="${APP_NAME}"
```

## Usage

Once the files are copied and `auth.php` is registered in `web.php`, the authentication routes become available in your Laravel application.

The system provides the core authentication flow including:

* Login
* Registration
* Email verification
* Email OTP verification
* Forgot password
* Reset password

## Scalability

The authentication system is designed to be easy to extend.

You can add additional:

* User fields
* Authentication methods
* Verification methods
* Security checks
* Profile information
* User-related features

without having to rebuild the authentication system from scratch.

## Tech Stack

* **Laravel**
* **PHP**
* **Blade**
* **Laravel Web**
* **MySQL / SQLite / PostgreSQL**

## License

This project is open source and can be used and modified for your own Laravel applications.
