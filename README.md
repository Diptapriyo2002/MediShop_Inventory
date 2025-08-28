# MediShop_Inventory

The **Medicine Shop Inventory Management System** is a Django-based web application designed to simplify and automate the management of medicines in a pharmacy or medical store. The system allows shop owners to:

* **Track medicines** purchased from wholesalers and sold to customers.
* **Update stock automatically** in real-time whenever a purchase or sale is recorded.
* **Monitor stock levels** and get alerts for low stock medicines.
* **Generate reports** on total purchases, sales, and profits.
* Manage all operations from a **simple and user-friendly web interface**.

This project was built using **Python (Django framework)** for the backend, **HTML/CSS/JavaScript** for the frontend, and **MySQL (via XAMPP)** as the database.
 Add and manage medicines
 Record purchases from wholesalers
 Record sales to customers
 Auto-update stock after purchase/sale
 Low stock alerts
 Reports for purchases, sales, and profits


## ⚙️ Technologies Used

* **Backend:** Django (Python)
* **Frontend:** HTML, CSS, JavaScript, Bootstrap
* **Database:** MySQL (XAMPP)
* **ORM:** Django ORM
* **Driver:** `mysqlclient` (Python connector for MySQL)

## How to Run the Project

### 1. Prerequisites

Make sure you have installed:

* Python 3.9+
* pip (Python package manager)
* Django (latest stable version)
* MySQL server (via XAMPP)
* `mysqlclient` package for Django-MySQL connection


### 2. Configure Database

1. Open **XAMPP Control Panel** and start **Apache** and **MySQL**.
2. Create a database in MySQL:

DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME': 'medicine_shop',
        'USER': 'root',
        'PASSWORD': '',
        'HOST': 'localhost',
        'PORT': '3306',
        'OPTIONS': {
            'init_command': "SET sql_mode='STRICT_TRANS_TABLES'",
        }
    }
}

### 3. Run Migrations

python manage.py makemigrations
python manage.py migrate

### 4. Run the Server

python manage.py runserver


