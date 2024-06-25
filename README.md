# 🧪 PostgreSQL Periodic Table Database

This project provides a PostgreSQL database containing basic information about chemical elements, including their physical properties and classifications.

## 📁 Project Structure

The project includes an SQL file that can be used to create the "periodic_table" database in PostgreSQL. This file contains table definitions for storing elements (`elements`), properties (`properties`), and types (`types`).

## 🌟 Key Features

### Tables

1. **elements**: Holds information about each element, including atomic number, symbol, and name.
2. **properties**: Stores physical properties of elements such as atomic mass, melting point, and boiling point.
3. **types**: Defines types of elements such as metal, metalloid, and non-metal.

### Constraints and Keys

- Primary key and unique constraints have been set on tables to ensure data integrity.
- Foreign key (`FOREIGN KEY`) relationships are defined between `elements` and `properties`, as well as between `properties` and `types`.

### 📊 SQL Queries

A bash script (`element.sh`) is included that allows querying the database to retrieve detailed information about a specific element by its atomic number or symbol.

## 🛠️ Using the Script

The `element.sh` script takes an argument which can be either an atomic number or an element symbol. It returns detailed information about the queried element, including atomic number, name, symbol, type, atomic mass, melting point, and boiling point.

### Example usage:

```bash
./element.sh 6

./element.sh "Carbon"
```

## ⚙️ Requirements

PostgreSQL version 12.17 or higher.
PostgreSQL user with adequate permissions to create databases and tables.

## 🚀 Setup

Ensure PostgreSQL is installed and configured.
Execute periodic_table.sql using psql or a compatible tool.

## 🤝 Contributions

Contributions are welcome. If you wish to improve this project, please submit a pull request.