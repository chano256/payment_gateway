## Project

This is a fullstack payment gateway with Laravel backend and Vue frontend.

## Api Deployment Guide

The api contains routes to initiate payments and check their statuses. The api requires the following: 

1. PHP ≥8.2
2. Composer
3. MySQL (or other RDBMS)


## Frontend Deployment Guide

The frontend is a single-page application built with Vue js. It requires the following:
1. Node.js ≥16
2. NPM

## Getting Started
Clone the project from github and run the following commands:

```bash
git clone https://github.com/chano256/payment_gateway.git
cd payment_gateway
```
Lets set up the backend

Modify the env file to match the created database with db name, username and password then run the following commands:

```bash
cd api
cp .env.example .env
php artisan key:generate
composer install
php artisan migrate
php artisan serve
```

Then lets set up the frontend

Run the following commands:

```bash
cd frontend
npm install
npm run dev
```
Note: For production, we shall use 
```bash
npm run build
```

### Premium Partners
- DFCU Bank

## Contributing
Allan Ochan