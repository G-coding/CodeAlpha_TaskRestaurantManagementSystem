🍴 Restaurant

  A simple microservices-based restaurant management dashboard built with React (frontend) and Django REST Framework (backend).
  The dashboard allows managing Menu Items, Orders, Reservations, and Inventory in a single UI.

🚀 Features

  📋 Menu Management — View restaurant menu items with name, description, and price.
  🛒 Orders Management — View customer orders and their statuses.
  📅 Reservations — View table reservations with customer details.
  📦 Inventory — Track available items, quantities, and units.
  🔗 Microservices Architecture — Each module (Menu, Orders, Reservations, Inventory) is powered by its own Django REST API.
  🎨 React Frontend — Clean, modular UI with navigation.

🛠️ Tech Stack

  Frontend: React, React Router
  Backend: Django + Django REST Framework (microservices)
  Database: MySQL

📂 Project Layout

    restaurant-dashboard/
  │
  ├── backend/
  │   ├── menu_service/
  │   ├── order_service/
  │   ├── reservation_service/
  │   ├── inventory_service/
  │   └── ...
  │
  ├── frontend/  (React app)
  │   ├── src/
  │   │   ├── components/
  │   │   │   ├── MenuItems.js
  │   │   │   ├── Orders.js
  │   │   │   ├── Reservations.js
  │   │   │   └── Inventory.js
  │   │   └── App.js
  │   └── package.json
  │
  └── README.md

⚙️ Installation

  1️⃣ Clone Repository
  git clone https://github.com/your-username/restaurant-dashboard.git
  cd restaurant-dashboard

  2️⃣ Backend Setup (Django Services)
  Each microservice (menu, orders, reservations, inventory) runs separately.
  Inside each service folder:
  pip install -r requirements.txt
  python manage.py makemigrations
  python manage.py migrate
  python manage.py runserver <port>
  Example:
  Menu Service → 127.0.0.1:8001
  Orders Service → 127.0.0.1:8002
  Reservation Service → 127.0.0.1:8003
  Inventory Service → 127.0.0.1:8004

  3️⃣ Frontend Setup (React)
  Go to the frontend folder:
  cd frontend
  npm install
  npm start
  The app will run on:
  👉 http://localhost:3000

🔗 API Endpoints

  Menu Service → http://127.0.0.1:8001/api/menu/
  Orders Service → http://127.0.0.1:8002/api/order/
  Reservations Service → http://127.0.0.1:8003/api/reservation/
  Inventory Service → http://127.0.0.1:8004/api/inventory/
