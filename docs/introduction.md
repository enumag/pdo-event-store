# Introduction

The PDO Event Store is an implementation of [prooph/event-store](https://github.com/prooph/event-store) that supports
MySQL and MariaDB as well as PostgreSQL.

## Video Introduction

[![Prooph Event Store v7](https://img.youtube.com/vi/QhpDIqYQzg0/0.jpg)](https://www.youtube.com/watch?v=QhpDIqYQzg0)

## Installation

```php
composer require prooph/pdo-event-store
```

## Requirements

- PHP >= 7.1
- PDO_MySQL Extension or PDO_PGSQL Extension

For MariaDB you need server vesion >= 10.2.6.
For MySQL you need server version >= 5.7.9.
For Postgres you need server version >= 9.4.

## Setup

For MariaDB run the script in `scripts/mariadb/01_event_streams_table.sql` on your server.

For MySQL run the script in `scripts/mysql/01_event_streams_table.sql` on your server.

For Postgres run the script in `scripts/postgres/01_event_streams_table.sql` on your server.

This will setup the required event streams table.

If you want to use the projections, run additionally the scripts `scripts/mariadb/02_projections_table.sql`
(for MariaDB), `scripts/mysql/02_projections_table.sql` (for MySQL) or
`scripts/postgres/02_projections_table.sql` (for Postgres) on your server.