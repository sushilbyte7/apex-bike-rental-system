# Apex Bike Rental System

A web-based bike rental platform built with PHP and MySQL. Users can browse and search bikes, book a rental, and manage their bookings; an admin panel manages vehicles, brands, bookings and users.

Built as a BCA final-year project (session 2021–2024).

## Features

- User registration and login
- Bike listing with search and brand filtering
- Bike details page and booking flow
- My Bookings, profile management and password update
- Testimonials and contact queries
- Admin panel: manage vehicles, brands, bookings, registered users, testimonials and site pages
- Razorpay payment library included under `razorpay/`

## Tech Stack

- HTML, CSS, JavaScript, Bootstrap
- PHP
- MySQL

## Setup (local, XAMPP)

1. Copy this folder into your web server root (for example `htdocs/` in XAMPP).
2. Create a MySQL database named `bikerental`.
3. Import `sqlfile/bikerental.sql` into that database (phpMyAdmin → Import).
4. Database settings are in `includes/config.php` — default is host `localhost`, user `root`, empty password (XAMPP default). Change these for any real deployment.
5. Open `http://localhost/<folder-name>/` in a browser.
   Admin panel: `http://localhost/<folder-name>/admin/`

## Project Structure

```
├── index.php            # Home page
├── bike-listing.php     # All bikes
├── vehical-details.php  # Bike details + booking
├── my-booking.php       # User bookings
├── admin/               # Admin panel
├── includes/            # Header, footer, DB config
├── assets/              # CSS, JS, images, fonts
├── razorpay/            # Razorpay PHP library
└── sqlfile/             # Database dump (schema + sample data)
```

## Note

The SQL dump ships with the sample/demo data that came with the project (sample users, vehicles and testimonials) so the site runs out of the box. Vehicle and site images are added separately in the repository's image folders under `assets/images/` and `admin/img/`.
