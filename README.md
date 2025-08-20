
# CleanArchitecture Backend
This is the backend system for a health management application, built as part of a recruitment assignment.
---

## Project Structure

- `CleanArchitecture.API` – Entry point, controllers, program configuration
- `CleanArchitecture.Application` – Business logic, service interfaces, DTOs
- `CleanArchitecture.Domain` – Entity models, enums
- `CleanArchitecture.Infrastructure` – EF Core, database context, repositories
- `CleanArchitecture.Test` – Unit test

---

## Tech Stack

- ASP.NET Core 9
- Entity Framework Core
- MySQL
- Clean Architecture
- Scalar

---

## How to Run

1. **Setup MySQL database**
   - Create database `CleanArchitecture`
   - Update connection string in `CleanArchitecture.API/appsettings.Development.json`

2. **Apply migration**
   ```bash
   dotnet ef database update -p CleanArchitecture.Infrastructure -s CleanArchitecture.API
   ```

3. **Run API**
   ```bash
   dotnet run --project CleanArchitecture.API
   ```

4. **Test in browser**
   - Scalar UI: `https://localhost:7157/scalar/v1`

---

## Database Schema

See `/Documents/CleanArchitecture - DB table.html`

---

## 📡 API List

Details: see `/Documents/api-spec.md`

## Author
Bùi Quốc Việt  