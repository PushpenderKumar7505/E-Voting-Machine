# 🗳️ E-Voting Machine

A web-based **Electronic Voting Management System** built with PHP and MySQL, designed to conduct secure, organized online elections with an admin-controlled interface.

---

## 📌 Overview

This system provides a complete voting platform where an administrator can set up elections, manage candidates, register voters, and view real-time results — all through a clean web interface. Voters can log in securely and cast their votes for their preferred candidates within defined categories.

---

## ✨ Features

- **Admin Dashboard** — Full control over elections, voters, and results
- **Voter Login & Authentication** — Secure login system for registered voters
- **Election Categories** — Organize candidates into separate voting categories (e.g., President, Secretary)
- **Candidate Management** — Add, edit, or remove candidates and their profiles
- **User Management** — Register and manage voter accounts
- **Live Vote Tracking** — View voting standings and results in real time
- **Vote Sheet Generation** — Printable vote summary reports
- **AJAX-Powered UI** — Smooth, responsive interactions without page reloads

---

## 🛠️ Tech Stack

| Layer       | Technology          |
|-------------|---------------------|
| Backend     | PHP (Core)          |
| Database    | MySQL               |
| Frontend    | HTML, CSS, JavaScript (AJAX) |
| Server      | Apache (XAMPP/WAMP) |

---

## 📂 Project Structure

```
E-Voting-Machine/
│
├── index.php              # Entry point / landing page
├── login.php              # Voter login page
├── home.php               # Voter dashboard after login
├── voting.php             # Voting interface
├── voting_list.php        # List of active elections
├── vote_sheet.php         # Vote summary / ballot sheet
├── view_vote.php          # Result viewer
│
├── admin_class.php        # Admin business logic
├── ajax.php               # AJAX request handler
├── db_connect.php         # Database connection config
│
├── categories.php         # Election category management
├── manage_catset.php      # Category settings
├── manage_opt.php         # Candidate/option management
├── manage_user.php        # Voter user management
├── manage_voting.php      # Election/voting session management
├── users.php              # User listing
│
├── header.php             # Common header template
├── navbar.php             # Navigation bar
├── topbar.php             # Top navigation bar
├── files.php              # File includes/utilities
│
└── standings.PNG          # Sample result screenshot
```

---

## ⚙️ Setup & Installation

### Prerequisites
- PHP 7.x or higher
- MySQL 5.x or higher
- Apache server (XAMPP or WAMP recommended)

### Steps

**1. Clone the repository**
```bash
git clone https://github.com/PushpenderKumar7505/E-Voting-Machine.git
```

**2. Move to server root**

Copy the project folder into your server's `htdocs` (XAMPP) or `www` (WAMP) directory.

**3. Import the database**

Open **phpMyAdmin**, create a new database (e.g., `evoting_db`), and import the SQL file included in `Voting-Management-System.zip`.

**4. Configure database connection**

Edit `db_connect.php` with your local credentials:
```php
$conn = new mysqli("localhost", "root", "", "evoting_db");
```

**5. Run the application**

Start Apache and MySQL from your control panel, then open:
```
http://localhost/E-Voting-Machine/
```

---

## 🖥️ Usage

**Admin**
- Log in via the admin panel
- Create election categories and add candidates
- Register voter accounts
- Open/close voting sessions
- View real-time standings and results

**Voter**
- Log in with registered credentials
- View active elections
- Cast vote for preferred candidate
- View voting confirmation

---

## 📸 Screenshot

![Voting Standings](standings.PNG)

---

## 🔒 Security Notes

- Each registered voter can vote only once per election category
- Session-based authentication is enforced throughout the application
- Admin and voter roles are separated

---

## 👤 Author

**Pushpender Kumar**
- GitHub: [@PushpenderKumar7505](https://github.com/PushpenderKumar7505)
- B.Tech CSE | GLA University, Mathura
- Aspiring DevOps & Cloud Engineer

---

## 📄 License

This project is open source and available for educational purposes.
