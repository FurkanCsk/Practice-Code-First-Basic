# Patika Code First - EF Core Example

This project demonstrates how to create a database using the **Code First** approach with **Entity Framework Core**. The project includes two independent tables: **Movies** and **Games**, which store relevant information for movies and games.

## Database Details

- **Database Name**: PatikaCodeFirstDb1
- **Tables**:
  - `Movies`
  - `Games`

## Movie Table Columns:
- **Id**: Primary Key, auto-incremented integer.
- **Title**: String, the title of the movie.
- **Genre**: String, the genre of the movie (e.g., "Action", "Comedy").
- **ReleaseYear**: Integer, the release year of the movie.

## Game Table Columns:
- **Id**: Primary Key, auto-incremented integer.
- **Name**: String, the name of the game.
- **Platform**: String, the platform the game is played on (e.g., "PC", "PlayStation").
- **Rating**: Decimal, the rating of the game (0-10 scale).

## Context Class

- **PatikaFirstDbContext**: Represents the session with the database and is used to query and save instances of the entities.
  
## Instructions

1. Define your entity classes (`Movie` and `Game`).
2. Create the `PatikaFirstDbContext` class to manage the connection and DbSets for `Movies` and `Games`.
3. Use migrations to create the database:
   - Run `dotnet ef migrations add InitialCreate`.
   - Then run `dotnet ef database update` to apply the migration.

This setup will automatically create the database and its tables based on the provided entities.
