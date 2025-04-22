# Laravel REST API – Task Manager

This is a simple REST API built with Laravel to manage tasks. It includes full CRUD operations with JSON responses and clean RESTful routing.

## 🔧 Features

- List all tasks
- Show a single task
- Create new task
- Update existing task
- Delete task
- API Resource structure
- Optional: Add token-based auth (e.g. Laravel Sanctum)

## 🧱 Tech Stack

- Laravel 10+
- MySQL
- RESTful architecture
- Laravel API Resources

---

## 🚀 Getting Started

### 1. Clone the Repo

```bash
git clone https://github.com/your-username/laravel-rest-api.git
cd laravel-rest-api
```

### 2. Install Dependencies

```bash
composer install
```

### 3. Create `.env` File

Copy `.env.example` to `.env` and update DB credentials.

```bash
cp .env.example .env
php artisan key:generate
```

### 4. Setup Database

```bash
php artisan migrate
```

### 5. Seed Example Tasks (optional)

```bash
php artisan tinker
>>> \App\Models\Task::factory()->count(5)->create();
```

---

## 📦 API Endpoints

| Method | Endpoint         | Description              |
|--------|------------------|--------------------------|
| GET    | /api/tasks       | Get all tasks            |
| GET    | /api/tasks/{id}  | Get single task          |
| POST   | /api/tasks       | Create new task          |
| PUT    | /api/tasks/{id}  | Update existing task     |
| DELETE | /api/tasks/{id}  | Delete task              |

### Sample JSON Request

```json
{
  "title": "Write documentation",
  "description": "Finish API docs and push to GitHub",
  "status": "pending"
}
```

---

## 📬 Contact

Want a more advanced API?  
Let’s connect → [codewithwaqas.com](https://codewithwaqas.com)
