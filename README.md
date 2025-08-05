# 🧪 Laravel Tinker Playground

Laravel Tinker is a powerful REPL for testing your Laravel code interactively.
This mini project helps beginners understand how to use Tinker effectively with real examples.

## 🚀 Getting Started

### 1. Clone the Repo

```bash
git clone https://github.com/yourusername/laravel-tinker-playground.git
cd laravel-tinker-playground
composer install
```

### 2. Setup Environment

```bash
cp .env.example .env
php artisan key:generate
```

Make sure to configure your `.env` file for a local MySQL setup.

### 3. Run Migrations & Seeders

```bash
php artisan migrate
php artisan db:seed
```

### 4. Enter Tinker

```bash
php artisan tinker
```

## 📌 What You’ll Learn

- Basic Eloquent Queries: `User::all()`, `Post::find(1)`
- Creating Records using `User::create()`
- Using Factories
- Relationship Testing: `User::find(1)->posts`, `Post::find(1)->user`
- Simulating Auth: `auth()->login(User::find(1))`

## 📦 Models Included

- User (hasMany Posts)
- Post (belongsTo User)

## 🎓 Perfect For

- Laravel beginners learning Eloquent
- Experimenting before writing controllers
- Debugging model logic