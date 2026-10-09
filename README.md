# Gym Management System

Web application for running a gym, built with Laravel 9. It has a public site for visitors and a dashboard with three roles: admin, coach and client.

## Features

- **Public site**: home, services, working hours, pricing, blog, sign-in and sign-up
- **Training packages**: create and manage packages; clients buy them with Stripe Checkout
- **Training sessions**: schedule sessions, assign coaches, and let clients attend
- **Coaches**: separate coach login, profile and password reset
- **Attendance**: session attendance records
- **Revenue**: income from purchased packages
- **Users**: manage users, ban and unban accounts
- **Blog**: admin-managed posts shown on the public site
- **Access control**: admin, coach and client roles

## Tech stack

PHP 8, Laravel 9, MySQL, Blade, AdminLTE 3, Spatie Laravel Permission, Laravel Ban, Yajra DataTables, Stripe

## Getting started

```bash
git clone https://github.com/belalyasin/gym-management-system.git
cd gym-management-system
composer install
npm install && npm run dev
cp .env.example .env      # set the DB_* values and your Stripe keys
php artisan key:generate
php artisan migrate --seed
php artisan serve
```
