# 📝 To-Do List Management App

<div align="center">

Homepage
<img width="1886" height="912" alt="Landing page" src="https://github.com/user-attachments/assets/f44c855a-4a9f-45b4-8ea3-795725bf080a" />

Edit Page
<img width="1868" height="912" alt="Edit page" src="https://github.com/user-attachments/assets/2af69bf5-1818-41f8-b705-c6d2bcaca995" />

Completed
<img width="907" height="897" alt="Completed" src="https://github.com/user-attachments/assets/cec4c0b0-a6c1-4710-b3a8-909c9eaa9052" />



**A clean, modern To-Do List web application built with Laravel.**  
Stay organized. Get things done. 🚀

</div>

---

## ✨ Features

| Feature | Description |
|---|---|
| ➕ **Add Tasks** | Create tasks with title, description, due date and priority |
| ✏️ **Edit Tasks** | Update any task details anytime |
| 🗑️ **Delete Tasks** | Remove tasks with a confirmation prompt |
| ✅ **Toggle Status** | Switch tasks between Pending and Completed instantly |
| 🔍 **Filter Tasks** | Filter by All, Pending, or Completed status |
| 📊 **Live Stats** | See count of pending and completed tasks at a glance |
| 🎨 **Beautiful UI** | Modern gradient design with smooth hover effects |

---

## 🖥️ Screenshots

> Home Page — Add tasks on the left, view all tasks on the right with filter tabs and live stats.

> Edit Page — Clean form to update task title, description, due date, priority and status.

---

## 🛠️ Tech Stack

- **Backend** — Laravel 11, PHP 8.1+
- **Database** — MySQL
- **Frontend** — Bootstrap 5, Font Awesome 6, Google Fonts (Poppins)
- **Tools** — Composer, XAMPP, phpMyAdmin

---

## ⚙️ Installation & Setup

Follow these steps to run the project locally:

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/todo-app.git
cd todo-app
```

### 2. Install Dependencies

```bash
composer install
```

### 3. Create Environment File

```bash
cp .env.example .env
```

### 4. Configure Database

Open `.env` and update these lines:

```env
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=todo_db
DB_USERNAME=root
DB_PASSWORD=
```

### 5. Generate App Key

```bash
php artisan key:generate
```

### 6. Run Migrations

```bash
php artisan migrate
```

### 7. Start the Server

```bash
php artisan serve
```

### 8. Open in Browser

```
http://127.0.0.1:8000
```

---

## 📁 Project Structure

```
todo-app/
├── app/
│   ├── Http/
│   │   └── Controllers/
│   │       └── TaskController.php   # Handles all task logic
│   └── Models/
│       └── Task.php                 # Task model
├── database/
│   └── migrations/
│       └── xxxx_create_tasks_table.php
├── resources/
│   └── views/
│       ├── layouts/
│       │   └── app.blade.php        # Main layout file
│       └── tasks/
│           ├── index.blade.php      # Home page
│           └── edit.blade.php       # Edit task page
└── routes/
    └── web.php                      # All routes
```

---

## 🗄️ Database Schema

**Table: `tasks`**

| Column | Type | Description |
|---|---|---|
| `id` | BIGINT | Primary key, auto increment |
| `title` | VARCHAR | Task title |
| `description` | TEXT | Task description (nullable) |
| `due_date` | DATE | Task due date (nullable) |
| `priority` | ENUM | High / Medium / Low |
| `status` | ENUM | Pending / Completed |
| `created_at` | TIMESTAMP | Auto generated |
| `updated_at` | TIMESTAMP | Auto generated |

---

## 🔗 Routes

| Method | URL | Action |
|---|---|---|
| GET | `/` | Show all tasks |
| POST | `/tasks` | Store new task |
| GET | `/tasks/{id}/edit` | Show edit form |
| PUT | `/tasks/{id}` | Update task |
| DELETE | `/tasks/{id}` | Delete task |
| PATCH | `/tasks/{id}/toggle` | Toggle task status |

---

## 👨‍💻 Author

**Your Name**  
📧 your-email@example.com  
🌐 [github.com/your-username](https://github.com/your-username)

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

<div align="center">

Made with ❤️ using Laravel  
⭐ Star this repo if you found it helpful!

</div>
