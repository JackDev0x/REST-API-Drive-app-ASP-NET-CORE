# Internet platform for automotive advertising – ASP.NET Core API

This project is a fully-featured web platform, designed for listing and browsing passenger car advertisements. In addition to the core functionality of a car classifieds portal, the platform introduces **user interaction features** such as **comments and discussions under each listing**.

Key features include:

- User registration and authentication with **JWT tokens**
- Secure backend built with **ASP.NET Core** and **EF Core (Code First)**
- Relational **database integration** via dependency injection (connection string configuration)
- Hybrid mapping strategy: **AutoMapper** for simple transformations, manual mapping for custom logic
- **Azure Blob Storage** integration for uploading and serving car images
- Modular API architecture with partial separation of concerns (controllers with selected service classes)
- Role-based access and authentication for protected endpoints
- Users can **create, edit, delete** their listings
- Visitors can **browse, search, filter** car ads
- Each listing supports **comment threads and discussions**
- **Braintree sandbox integration** simulates online payments for posting new advertisements
---

## Technologies Used

- ASP.NET Core Web API  
- Entity Framework Core (Code First)  
- SQL Server  
- Azure Blob Storage  
- Braintree Sandbox (test payments)  
- JWT Authentication  
- Dependency Injection
- AutoMapper (object-object mapping)
- Swagger for API documentation

---

## Project Structure

- `Controllers` – API controllers  
- `Services` – Business logic
- `Models` – DTOs
- `Entities` - Data models and EF _DbContext_
- `Migrations` - Entity Framework Core migration classes 

---

⚠️ Note: This project depends on external services (Azure Blob Storage, Braintree) and requires local secrets configuration. The `appsettings.json` file is excluded from the repository for security reasons, so the application may not run out-of-the-box for third parties. However, the full source code and architecture are available for review.


