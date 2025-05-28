
# SQLx CLI Installation
To install the [SQLx CLI](https://crates.io/crates/sqlx-cli) with support for PostgreSQL, you can use the following command:
```sh
cargo install sqlx-cli --no-default-features --features native-tls,postgres
```

# Migrations
To manage database migrations using SQLx, you can use the `sqlx migrate` command. First, ensure you have a directory for your migrations, typically named `migrations`. You can create this directory and add a migration file with the following command:
```sh
sqlx migrate add tables
```

# Create database
To create a PostgreSQL database, you can use the `createdb` command. Replace `your_database_name` with the desired name for your database:
```sh
sqlx database create
```

# Run migrations
To run the migrations you have created, use the following command:
```sh
sqlx migrate run
```
# List tables
```sh
file_share=# \d
List of relations
Schema |       Name       | Type  |  Owner
--------+------------------+-------+----------
public | _sqlx_migrations | table | postgres
public | files            | table | postgres
public | shared_links     | table | postgres
public | users            | table | postgres
(4 rows)
```