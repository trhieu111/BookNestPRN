# BookNestPRN

**BookNestPRN** is a comprehensive Bookstore Management System designed for efficient management of book inventories, orders, and user activities. Built with a multi-layered architecture, the system supports robust CRUD operations and is suitable for both educational and real-world small business use cases.

---

## Table of Contents

- [Features](#features)
- [Technologies Used](#technologies-used)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
  - [Database Setup](#database-setup)
  - [Running the Application](#running-the-application)
- [Project Structure](#project-structure)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

---

## Features

- User authentication & authorization (Admins, Users)
- Browse, search, and filter books
- Manage book inventory (CRUD operations)
- Manage customers and orders
- Shopping cart & checkout system
- Order history and details
- Responsive UI

---

## Technologies Used

- **Backend:** ASP.NET Core / C#  
- **Frontend:** ASP.NET MVC / Razor Pages  
- **Database:** SQL Server  
- **ORM:** Entity Framework Core  
- **Other:** Bootstrap, jQuery, LINQ

---

## Getting Started

### Prerequisites

- [.NET 6.0 SDK or later](https://dotnet.microsoft.com/download)
- [SQL Server](https://www.microsoft.com/en-us/sql-server/sql-server-downloads)
- An IDE such as [Visual Studio 2022](https://visualstudio.microsoft.com/vs/) or [Visual Studio Code](https://code.visualstudio.com/)

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/trhieu111/BookNestPRN.git
   cd BookNestPRN
   ```

2. **Configure the connection string:**
   - Open `appsettings.json` or the configuration file.
   - Update the `DefaultConnection` string to point to your SQL Server instance.

3. **Restore dependencies:**
   ```bash
   dotnet restore
   ```

### Database Setup

1. **Apply migrations and create the database:**
   ```bash
   dotnet ef database update
   ```
   *(Or use the Package Manager Console in Visual Studio)*

2. **Seed initial data:**  
   *(Check for a data seeder or SQL scripts in the repository and run as needed.)*

### Running the Application

- Start the application from Visual Studio (`F5`) or use:
  ```bash
  dotnet run
  ```
- Navigate to `https://localhost:5001` in your browser.

---

## Project Structure

```
BookNestPRN/
│
├── BookNestPRN/             # Main application code
│   ├── Controllers/         # MVC Controllers
│   ├── Models/              # Entity & View Models
│   ├── Views/               # Razor Views
│   ├── Data/                # DbContext and migrations
│   └── wwwroot/             # Static files (CSS, JS, images)
├── BookNestPRN.sln          # Solution file
└── README.md
```

---

## Usage

- **Admin** can manage books, categories, users, and view order reports.
- **Users** can register, login, browse books, add to cart, checkout, and view their order history.

---

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
