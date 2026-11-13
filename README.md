# Vargas Movies – ASP.NET Core MVC

A movie catalog web app built with **ASP.NET Core MVC** and **Entity Framework Core** for CSE 325 (.NET Software Development) at BYU-Idaho, Week 2.

Based on Microsoft's tutorial [Get started with ASP.NET Core MVC](https://learn.microsoft.com/en-us/aspnet/core/tutorials/first-mvc-app/start-mvc?view=aspnetcore-10.0&tabs=visual-studio-code), with additional features.

## Features

- Full CRUD for movies (create, read, update, delete)
- Search by title, filter by genre, and filter by release year
- Server-side and client-side validation with data annotations
- SQLite database managed with EF Core migrations, seeded with sample movies

### Customizations beyond the tutorial

1. App title changed to **Vargas Movies**
2. Added three of my own favorite movies to the seed data
3. Listing page heading changed from "Index" to **My Movies**
4. **Year selector**: filters movies released in the selected year or newer
5. Added padding to form inputs (`input`, `select`, `textarea`) throughout the app

## Tech stack

- .NET 10 / ASP.NET Core MVC
- Entity Framework Core 10 with SQLite
- Razor views, Bootstrap

## How to run

**Requirements:** [.NET 10 SDK](https://dotnet.microsoft.com/download/dotnet/10.0)

```bash
git clone https://github.com/cvargas306/mvc-movie-app.git
cd mvc-movie-app
dotnet run --launch-profile https
```

Then open **https://localhost:7230/Movies** (or click **Vargas Movies** in the navigation bar).

The SQLite database is created and seeded automatically on first run. No extra setup is needed.

> If the browser warns about the HTTPS certificate, run `dotnet dev-certs https --trust` once, or use the HTTP address shown in the terminal.

## Author

Carlos Vargas Badilla – [github.com/cvargas306](https://github.com/cvargas306)