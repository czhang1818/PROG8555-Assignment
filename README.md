# Product Catalog

An ASP.NET Core MVC application for managing products and categories with full CRUD functionality.

## Features

- **Category Management**: Create, view, edit, and delete product categories
- **Product Management**: Full CRUD operations with category assignment
- **SQL Server Database**: Entity Framework Core with LocalDB
- **Tag Helpers**: Modern ASP.NET Core UI components

## Technologies

- ASP.NET Core MVC (.NET 10)
- Entity Framework Core
- SQL Server LocalDB
- Bootstrap 5

## Project Structure

```
ProductCatalog/
├── Controllers/
│   ├── CategoryController.cs
│   ├── ProductController.cs
│   └── HomeController.cs
├── Models/
│   ├── Category.cs
│   └── Product.cs
├── Data/
│   └── AppDbContext.cs
├── Views/
│   ├── Category/
│   ├── Product/
│   ├── Home/
│   └── Shared/
└── Migrations/
```

## Database Schema

### Category

| Column       | Type   | Description              |
| ------------ | ------ | ------------------------ |
| Id           | int    | Primary key              |
| CategoryName | string | Category name (required) |

### Product

| Column       | Type    | Description             |
| ------------ | ------- | ----------------------- |
| Id           | int     | Primary key             |
| ProductName  | string  | Product name            |
| ProductPrice | decimal | Price                   |
| ImageUrl     | string  | Image path              |
| Description  | string  | Product description     |
| CategoryId   | int     | Foreign key to Category |

## Author

Chunxi Zhang

## License

This project is for educational purposes - PROG8555 Microsoft Web Technologies.
