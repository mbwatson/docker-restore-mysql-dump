# Dockerize Restored MySQL Dump with PHPMyAdmin

## What this accomplishes

With Docker Compose, you can spin up a `mysql` instance populated with the data in an `.sql` file from a previous MySQL database dump.

In addition, an instance of PHPMyAdmin will be started.

## How to use this

1. Put a dumped `.sql` file into the `db_data` directory.
2. Copy `.env.sample` to `.env` and add your desired settings, inclusing database credentials.
3. Execute `docker-compose up`.

Then MySQL should be accessible on the host's port 3306, and yo can access it from applications running on the host. Additionally, the PHPMyAdmin client will be accessible in your browser at `localhost:<PMACLIENT_PORT>`, where `PMACLIENT_PORT` is specified in your `.env` file.


