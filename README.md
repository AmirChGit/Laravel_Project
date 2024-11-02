# Laravel_Project

A Laravel-based API application with user authentication and management features.

## Overview

This project is built with Laravel, utilizing the Symfony Console component for command-line operations. It includes API routes for user registration, login, and management, employing Laravel Sanctum for authentication. The frontend is structured using Vite and React for a modern development experience.

## Features

- User authentication via signup and login endpoints.
- Secure user management with route protection using middleware.
- RESTful API for user data retrieval and management.
- Rate limiting for API requests to enhance security and performance.

## Getting Started

### Prerequisites

- PHP (>= 7.4)
- Composer
- Laravel (>= 8.x)
- Node.js and npm (for Vite + React)

### Installation

1. Clone the repository

Install PHP dependencies

composer install
Set up your .env file:

cp .env.example .env
php artisan key:generate
Install JavaScript dependencies:

npm install
Run database migrations:

php artisan migrate
Start the development server:

php artisan serve
In another terminal, run the Vite development server:

npm run dev
API Endpoints
Authentication
POST /signup - Register a new user.
POST /login - Log in an existing user.
POST /logout - Log out the authenticated user.
User Management (Authenticated Routes)
GET /user - Retrieve the authenticated user's details.
GET /users - List all users (requires authentication).
POST /users - Create a new user (requires authentication).
PUT /users/{user} - Update an existing user (requires authentication).
DELETE /users/{user} - Delete a user (requires authentication).
