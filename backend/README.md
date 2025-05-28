
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
